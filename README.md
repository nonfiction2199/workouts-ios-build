# Workouts — public iPhone build source

Clean source snapshot for **Workouts 1.7.0**, an independent native SwiftUI workout and food diary app. The original development repository remains private.

This repository contains build source and bundled reference assets, with no development Git history, user diaries, connection tokens, provider keys, signing certificates or personal photos. Attribution notices remain in the source archive. The large public-domain food database is generated from its pinned USDA release during the build.

GitHub Actions builds an unsigned ARM64 device IPA for Signulous using standard public-repository macOS runners. The workflow checks nutrition, the workout engine, theme contrast, native logging and release compilation. It also captures the updated logging, Levels and eight theme screens.

A build is ready only when native compilation and the selected checks pass. Download **Workouts-Signulous** from the successful run, unzip it, and sign the IPA with the existing bundle ID `app.sudais.workouts`. Install over the existing app to preserve data.

Pair Workouts 1.7.0 with the **Revision 10 local food service**. This update removes a contradictory photo-only prompt, rechecks empty photo results once within the request deadline, derives nutrient totals from per-100g estimates and pictured grams, and preserves measured weights as the highest-priority portion evidence. It refreshes themes and the front/back Levels map.

Photo recognition, grams and recipe nutrients remain estimates. Mock-provider tests verify handling and arithmetic, not real-model recognition accuracy. Simulator checks do not establish physical-camera depth accuracy or a pixel-perfect match to another app.
