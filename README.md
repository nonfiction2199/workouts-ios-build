# Workouts — public iPhone build source

Clean source snapshot for Workouts 1.5.0, an independent native SwiftUI workout and food diary app. The original development repository remains private. This repository contains build source and bundled reference assets, with no development Git history, user diaries, connection tokens, provider keys, signing certificates or personal photos.

GitHub Actions builds an unsigned ARM64 device IPA for installation through Signulous. Standard public-repository runners use GitHub's free Actions offering. Account restrictions may still need to be resolved with GitHub.

The workflow runs foundation checks, native nutrition/workout UI tests and a release compilation. Additional screenshot galleries are optional for manual runs. A build is ready only when native compilation and tests complete successfully. Download Workouts-Signulous from the successful run, unzip it, and sign the IPA with the existing bundle ID app.sudais.workouts. Install over the existing app to preserve data.

The bundled data, font and media attribution notices are retained inside Workouts-1.5.0-source.zip at Workouts-iOS/Workouts/Resources. Build dependencies remain pinned. The large public-domain food database is generated from its pinned USDA release during the build.


Workouts 1.5.0 adds text-only Describe, two-photo meal evidence, editable plates with totals, food addition/removal, fraction and known-calorie scaling, reusable recipes and source-aware review checks. Pair the IPA with the Revision 8 local service. Photo-derived weights and macros remain estimates; the update does not claim a measured accuracy score.
