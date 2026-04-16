# Trace Bench

This file is auto-updated by `.github/workflows/trace-bench.yml` after pull requests merge to `main`.

Each entry records the merged PR metadata plus the results from:

`scripts/bench-gh.sh --runs 5 --warmups 1`

Entries are keyed by merge commit SHA so reruns can skip duplicates.

<!-- trace-bench:29e5834111e8d5b0d719225a3175fef8901a5a69 -->
## 2026-04-03 08:22:04 UTC

- PR: [#1167](https://github.com/pingcap/agent-git-service/pull/1167) Add a repeatable gh CLI latency benchmark workflow
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-03T08:20:03Z
- Merge commit: `29e5834111e8d5b0d719225a3175fef8901a5a69`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/23939614123)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 52.178 | 51.992 | 54.187 | 50.872 | 54.187 |
| auth-status | 5 | 55.989 | 54.335 | 64.638 | 52.283 | 64.638 |
| auth-logout | 5 | 44.866 | 43.969 | 49.777 | 42.193 | 49.777 |
| repo-create | 5 | 121.327 | 121.111 | 126.488 | 116.902 | 126.488 |
| repo-view | 5 | 100.014 | 95.132 | 123.540 | 90.618 | 123.540 |
| repo-clone | 5 | 156.147 | 156.986 | 159.184 | 152.466 | 159.184 |
| issue-create | 5 | 156.899 | 157.907 | 159.769 | 151.048 | 159.769 |
| issue-list | 5 | 63.407 | 62.957 | 66.212 | 62.008 | 66.212 |
| issue-view | 5 | 87.046 | 87.585 | 90.709 | 83.325 | 90.709 |
| pr-create | 5 | 279.910 | 273.703 | 310.383 | 267.046 | 310.383 |
| pr-list | 5 | 78.230 | 77.401 | 80.917 | 76.486 | 80.917 |
| pr-view | 5 | 145.191 | 141.469 | 158.604 | 140.756 | 158.604 |
| pr-merge | 5 | 151.384 | 153.029 | 155.026 | 145.668 | 155.026 |
| workflow-list | 5 | 59.215 | 56.058 | 71.611 | 52.922 | 71.611 |
| workflow-run | 5 | 103.297 | 102.928 | 105.833 | 101.881 | 105.833 |
| run-view | 5 | 140.866 | 141.712 | 144.273 | 133.544 | 144.273 |


<!-- trace-bench:477f8c1b0785ab1d2a710f3b0caa65f71edc33bb -->
## 2026-04-07 04:06:39 UTC

- PR: [#1174](https://github.com/pingcap/agent-git-service/pull/1174) Provides analysis and optimization skills for trace_bench.md
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-07T04:04:27Z
- Merge commit: `477f8c1b0785ab1d2a710f3b0caa65f71edc33bb`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24063688406)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.154 | 50.977 | 54.267 | 47.291 | 54.267 |
| auth-status | 5 | 50.462 | 50.275 | 54.143 | 46.692 | 54.143 |
| auth-logout | 5 | 38.758 | 36.410 | 48.981 | 35.504 | 48.981 |
| repo-create | 5 | 120.025 | 118.518 | 127.393 | 116.762 | 127.393 |
| repo-view | 5 | 88.671 | 87.871 | 91.946 | 86.355 | 91.946 |
| repo-clone | 5 | 164.122 | 159.059 | 186.504 | 154.794 | 186.504 |
| issue-create | 5 | 154.328 | 153.253 | 158.749 | 149.037 | 158.749 |
| issue-list | 5 | 63.778 | 63.651 | 64.977 | 62.705 | 64.977 |
| issue-view | 5 | 87.928 | 85.844 | 97.764 | 84.317 | 97.764 |
| pr-create | 5 | 280.843 | 277.422 | 311.403 | 262.450 | 311.403 |
| pr-list | 5 | 84.607 | 82.883 | 90.057 | 81.540 | 90.057 |
| pr-view | 5 | 147.229 | 146.774 | 150.817 | 144.550 | 150.817 |
| pr-merge | 5 | 154.386 | 155.068 | 156.937 | 150.542 | 156.937 |
| workflow-list | 5 | 63.961 | 62.416 | 69.220 | 58.187 | 69.220 |
| workflow-run | 5 | 193.011 | 144.850 | 307.313 | 110.798 | 307.313 |
| run-view | 5 | 146.072 | 147.188 | 148.752 | 140.641 | 148.752 |


<!-- trace-bench:b982a8a22aa4fda2ec0416a2c554793a4688d6cf -->
## 2026-04-07 07:29:22 UTC

- PR: [#1182](https://github.com/pingcap/agent-git-service/pull/1182) perf: reduce redundant hot-path work in PR merge
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-07T07:27:02Z
- Merge commit: `b982a8a22aa4fda2ec0416a2c554793a4688d6cf`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24069686034)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 47.971 | 47.630 | 49.556 | 46.506 | 49.556 |
| auth-status | 5 | 49.366 | 49.363 | 50.629 | 48.347 | 50.629 |
| auth-logout | 5 | 40.863 | 38.277 | 47.074 | 35.795 | 47.074 |
| repo-create | 5 | 118.316 | 120.969 | 122.066 | 111.685 | 122.066 |
| repo-view | 5 | 100.449 | 96.567 | 122.890 | 91.993 | 122.890 |
| repo-clone | 5 | 166.183 | 165.659 | 171.798 | 161.452 | 171.798 |
| issue-create | 5 | 162.989 | 162.946 | 166.313 | 159.665 | 166.313 |
| issue-list | 5 | 77.844 | 70.849 | 97.152 | 65.929 | 97.152 |
| issue-view | 5 | 92.529 | 91.210 | 96.629 | 89.314 | 96.629 |
| pr-create | 5 | 282.806 | 279.005 | 301.645 | 276.007 | 301.645 |
| pr-list | 5 | 76.396 | 76.401 | 79.443 | 74.230 | 79.443 |
| pr-view | 5 | 146.706 | 146.460 | 151.205 | 140.925 | 151.205 |
| pr-merge | 5 | 144.890 | 141.351 | 155.914 | 140.575 | 155.914 |
| workflow-list | 5 | 56.706 | 56.040 | 59.293 | 54.912 | 59.293 |
| workflow-run | 5 | 109.478 | 105.019 | 128.223 | 103.078 | 128.223 |
| run-view | 5 | 145.100 | 144.200 | 155.081 | 137.007 | 155.081 |


<!-- trace-bench:5b17ea91bf66ca5d0b3db684c4fded861ef8ac70 -->
## 2026-04-07 07:31:22 UTC

- PR: [#1181](https://github.com/pingcap/agent-git-service/pull/1181) perf: add a lightweight response path for PR creation
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-07T07:27:16Z
- Merge commit: `5b17ea91bf66ca5d0b3db684c4fded861ef8ac70`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24069694299)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 53.089 | 52.879 | 54.986 | 51.638 | 54.986 |
| auth-status | 5 | 53.603 | 53.442 | 54.729 | 52.330 | 54.729 |
| auth-logout | 5 | 43.287 | 43.299 | 44.678 | 41.769 | 44.678 |
| repo-create | 5 | 126.023 | 127.370 | 132.986 | 115.999 | 132.986 |
| repo-view | 5 | 88.011 | 87.279 | 91.913 | 86.021 | 91.913 |
| repo-clone | 5 | 157.918 | 157.272 | 163.174 | 152.766 | 163.174 |
| issue-create | 5 | 156.780 | 156.201 | 161.002 | 151.911 | 161.002 |
| issue-list | 5 | 64.495 | 64.682 | 65.527 | 62.993 | 65.527 |
| issue-view | 5 | 92.560 | 86.496 | 115.000 | 84.682 | 115.000 |
| pr-create | 5 | 287.640 | 284.957 | 309.068 | 276.931 | 309.068 |
| pr-list | 5 | 80.011 | 79.497 | 87.615 | 76.194 | 87.615 |
| pr-view | 5 | 141.383 | 140.583 | 144.608 | 137.231 | 144.608 |
| pr-merge | 5 | 146.705 | 147.249 | 149.043 | 142.602 | 149.043 |
| workflow-list | 5 | 57.812 | 57.079 | 62.684 | 55.391 | 62.684 |
| workflow-run | 5 | 105.549 | 106.172 | 107.050 | 102.372 | 107.050 |
| run-view | 5 | 145.908 | 142.106 | 157.246 | 139.190 | 157.246 |


<!-- trace-bench:564d7d589aea647f7b6c893d4cd57545bd5843bb -->
## 2026-04-07 07:44:05 UTC

- PR: [#1183](https://github.com/pingcap/agent-git-service/pull/1183) perf: collapse immediate post-create DB work in issue creation
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-07T07:41:59Z
- Merge commit: `564d7d589aea647f7b6c893d4cd57545bd5843bb`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24070228401)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.810 | 50.145 | 57.863 | 48.649 | 57.863 |
| auth-status | 5 | 52.978 | 52.937 | 54.980 | 51.699 | 54.980 |
| auth-logout | 5 | 41.682 | 41.648 | 43.973 | 39.457 | 43.973 |
| repo-create | 5 | 120.313 | 119.176 | 124.928 | 117.335 | 124.928 |
| repo-view | 5 | 96.509 | 96.334 | 109.908 | 85.236 | 109.908 |
| repo-clone | 5 | 155.280 | 155.534 | 158.960 | 151.406 | 158.960 |
| issue-create | 5 | 146.523 | 146.628 | 149.459 | 141.949 | 149.459 |
| issue-list | 5 | 60.959 | 60.606 | 63.044 | 59.069 | 63.044 |
| issue-view | 5 | 84.840 | 85.610 | 87.963 | 80.692 | 87.963 |
| pr-create | 5 | 272.023 | 264.647 | 301.437 | 260.659 | 301.437 |
| pr-list | 5 | 72.658 | 71.402 | 76.159 | 70.661 | 76.159 |
| pr-view | 5 | 141.949 | 141.640 | 146.169 | 138.683 | 146.169 |
| pr-merge | 5 | 139.678 | 138.854 | 141.858 | 138.424 | 141.858 |
| workflow-list | 5 | 55.134 | 55.084 | 56.255 | 53.972 | 56.255 |
| workflow-run | 5 | 106.552 | 103.001 | 131.556 | 94.455 | 131.556 |
| run-view | 5 | 133.709 | 133.549 | 136.059 | 131.456 | 136.059 |


<!-- trace-bench:6b0ae6cef9c1f690bc78faf2a0369608b77ae9e0 -->
## 2026-04-07 08:54:47 UTC

- PR: [#1184](https://github.com/pingcap/agent-git-service/pull/1184) perf: trim repo stats work on repo create/view hot paths
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-07T08:52:44Z
- Merge commit: `6b0ae6cef9c1f690bc78faf2a0369608b77ae9e0`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24072936552)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 49.072 | 49.121 | 51.539 | 46.930 | 51.539 |
| auth-status | 5 | 49.471 | 48.927 | 52.289 | 47.348 | 52.289 |
| auth-logout | 5 | 38.188 | 37.582 | 40.507 | 36.244 | 40.507 |
| repo-create | 5 | 101.766 | 101.499 | 107.978 | 97.324 | 107.978 |
| repo-view | 5 | 93.860 | 96.080 | 97.339 | 88.936 | 97.339 |
| repo-clone | 5 | 169.192 | 164.110 | 197.879 | 156.645 | 197.879 |
| issue-create | 5 | 160.903 | 160.077 | 165.608 | 155.018 | 165.608 |
| issue-list | 5 | 74.259 | 74.225 | 82.295 | 67.375 | 82.295 |
| issue-view | 5 | 89.073 | 89.397 | 92.989 | 85.712 | 92.989 |
| pr-create | 5 | 282.019 | 281.584 | 283.651 | 280.358 | 283.651 |
| pr-list | 5 | 79.532 | 79.847 | 80.379 | 78.015 | 80.379 |
| pr-view | 5 | 141.861 | 142.324 | 144.655 | 136.749 | 144.655 |
| pr-merge | 5 | 145.705 | 143.141 | 152.226 | 139.733 | 152.226 |
| workflow-list | 5 | 58.068 | 57.177 | 61.970 | 55.369 | 61.970 |
| workflow-run | 5 | 239.480 | 104.517 | 781.577 | 98.815 | 781.577 |
| run-view | 5 | 143.020 | 139.385 | 160.780 | 132.143 | 160.780 |


<!-- trace-bench:2d5cc39292c8d28b62e5327d961538ccf04dcea4 -->
## 2026-04-07 12:10:52 UTC

- PR: [#1180](https://github.com/pingcap/agent-git-service/pull/1180) build(deps-dev): bump vite from 6.4.1 to 6.4.2 in /web
- PR resolution: resolved
- Author: @dependabot[bot]
- PR merged at: 2026-04-07T12:08:45Z
- Merge commit: `2d5cc39292c8d28b62e5327d961538ccf04dcea4`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24080530074)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 57.919 | 56.587 | 63.568 | 54.134 | 63.568 |
| auth-status | 5 | 57.328 | 57.031 | 61.402 | 55.549 | 61.402 |
| auth-logout | 5 | 43.497 | 43.132 | 48.851 | 38.926 | 48.851 |
| repo-create | 5 | 112.750 | 112.828 | 114.582 | 110.393 | 114.582 |
| repo-view | 5 | 96.293 | 96.901 | 99.941 | 92.179 | 99.941 |
| repo-clone | 5 | 173.731 | 173.688 | 178.303 | 170.575 | 178.303 |
| issue-create | 5 | 163.660 | 165.395 | 168.620 | 157.234 | 168.620 |
| issue-list | 5 | 73.930 | 72.062 | 83.399 | 69.844 | 83.399 |
| issue-view | 5 | 108.804 | 100.258 | 146.660 | 94.477 | 146.660 |
| pr-create | 5 | 300.753 | 293.580 | 333.176 | 284.243 | 333.176 |
| pr-list | 5 | 79.116 | 77.419 | 82.670 | 76.735 | 82.670 |
| pr-view | 5 | 147.904 | 147.381 | 152.539 | 144.763 | 152.539 |
| pr-merge | 5 | 152.944 | 152.058 | 165.573 | 145.425 | 165.573 |
| workflow-list | 5 | 60.406 | 59.442 | 65.958 | 56.939 | 65.958 |
| workflow-run | 5 | 111.080 | 112.066 | 115.342 | 106.279 | 115.342 |
| run-view | 5 | 149.816 | 147.535 | 158.354 | 145.358 | 158.354 |


<!-- trace-bench:c20f40cdf24981a62a7dd0582dff54b24cd1a364 -->
## 2026-04-08 08:24:31 UTC

- PR: [#1187](https://github.com/pingcap/agent-git-service/pull/1187) fix: optimize repo-scoped search label filters
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-08T08:22:18Z
- Merge commit: `c20f40cdf24981a62a7dd0582dff54b24cd1a364`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24125487166)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 53.252 | 53.402 | 54.278 | 51.655 | 54.278 |
| auth-status | 5 | 55.510 | 53.563 | 63.778 | 51.934 | 63.778 |
| auth-logout | 5 | 42.618 | 42.482 | 44.959 | 40.950 | 44.959 |
| repo-create | 5 | 110.368 | 111.109 | 114.898 | 106.122 | 114.898 |
| repo-view | 5 | 104.878 | 98.037 | 127.558 | 97.061 | 127.558 |
| repo-clone | 5 | 158.188 | 158.425 | 162.417 | 153.913 | 162.417 |
| issue-create | 5 | 151.318 | 151.026 | 154.457 | 148.637 | 154.457 |
| issue-list | 5 | 65.428 | 65.918 | 69.682 | 60.777 | 69.682 |
| issue-view | 5 | 87.770 | 87.105 | 92.376 | 84.362 | 92.376 |
| pr-create | 5 | 277.295 | 280.226 | 284.891 | 270.131 | 284.891 |
| pr-list | 5 | 78.064 | 78.143 | 79.893 | 75.286 | 79.893 |
| pr-view | 5 | 143.501 | 141.658 | 148.025 | 139.456 | 148.025 |
| pr-merge | 5 | 142.892 | 142.164 | 145.389 | 141.586 | 145.389 |
| workflow-list | 5 | 62.768 | 59.939 | 73.787 | 56.621 | 73.787 |
| workflow-run | 5 | 112.425 | 109.673 | 128.678 | 97.660 | 128.678 |
| run-view | 5 | 139.268 | 139.406 | 142.865 | 135.393 | 142.865 |


<!-- trace-bench:2c49fb4c59a8903ce360ccd0c5acb1224aae6aa6 -->
## 2026-04-08 09:08:29 UTC

- PR: [#1186](https://github.com/pingcap/agent-git-service/pull/1186) feat: remove default labels for repo creation
- PR resolution: resolved
- Author: @Icemap
- PR merged at: 2026-04-08T09:06:26Z
- Merge commit: `2c49fb4c59a8903ce360ccd0c5acb1224aae6aa6`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24127326006)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 54.775 | 54.878 | 57.950 | 52.951 | 57.950 |
| auth-status | 5 | 56.152 | 54.844 | 59.843 | 54.387 | 59.843 |
| auth-logout | 5 | 43.718 | 43.698 | 44.837 | 42.969 | 44.837 |
| repo-create | 5 | 67.135 | 66.874 | 68.686 | 65.939 | 68.686 |
| repo-view | 5 | 96.322 | 95.258 | 99.549 | 93.175 | 99.549 |
| repo-clone | 5 | 167.691 | 170.045 | 180.663 | 156.818 | 180.663 |
| issue-create | 5 | 147.910 | 147.359 | 151.833 | 145.584 | 151.833 |
| issue-list | 5 | 62.699 | 62.222 | 64.678 | 61.353 | 64.678 |
| issue-view | 5 | 83.956 | 84.208 | 86.087 | 81.883 | 86.087 |
| pr-create | 5 | 268.805 | 268.597 | 272.837 | 266.184 | 272.837 |
| pr-list | 5 | 78.856 | 79.589 | 81.323 | 73.516 | 81.323 |
| pr-view | 5 | 146.685 | 142.532 | 164.810 | 139.704 | 164.810 |
| pr-merge | 5 | 148.100 | 142.828 | 167.232 | 139.392 | 167.232 |
| workflow-list | 5 | 54.855 | 55.078 | 55.661 | 53.288 | 55.661 |
| workflow-run | 5 | 100.863 | 99.574 | 106.721 | 97.609 | 106.721 |
| run-view | 5 | 138.127 | 134.084 | 158.782 | 130.961 | 158.782 |


<!-- trace-bench:16820648e3cd589ecb90d17642c006b0e9f02b6d -->
## 2026-04-08 21:10:40 UTC

- PR: [#1188](https://github.com/pingcap/agent-git-service/pull/1188) build(deps-dev): bump basic-ftp from 5.2.0 to 5.2.1 in /web
- PR resolution: resolved
- Author: @dependabot[bot]
- PR merged at: 2026-04-08T21:08:17Z
- Merge commit: `16820648e3cd589ecb90d17642c006b0e9f02b6d`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24158807250)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.252 | 49.795 | 56.039 | 48.189 | 56.039 |
| auth-status | 5 | 50.331 | 50.600 | 51.549 | 49.321 | 51.549 |
| auth-logout | 5 | 38.931 | 40.024 | 42.175 | 35.079 | 42.175 |
| repo-create | 5 | 61.382 | 59.948 | 65.116 | 59.263 | 65.116 |
| repo-view | 5 | 87.022 | 86.695 | 89.910 | 84.957 | 89.910 |
| repo-clone | 5 | 158.791 | 158.595 | 161.212 | 155.369 | 161.212 |
| issue-create | 5 | 149.599 | 150.433 | 153.670 | 143.147 | 153.670 |
| issue-list | 5 | 63.942 | 64.467 | 65.139 | 61.489 | 65.139 |
| issue-view | 5 | 85.026 | 85.333 | 87.566 | 82.449 | 87.566 |
| pr-create | 5 | 273.828 | 272.916 | 280.421 | 269.836 | 280.421 |
| pr-list | 5 | 75.289 | 74.898 | 79.808 | 72.862 | 79.808 |
| pr-view | 5 | 150.901 | 147.303 | 173.676 | 137.177 | 173.676 |
| pr-merge | 5 | 159.848 | 152.328 | 195.543 | 147.410 | 195.543 |
| workflow-list | 5 | 62.008 | 62.049 | 63.134 | 60.552 | 63.134 |
| workflow-run | 5 | 106.380 | 105.695 | 110.188 | 100.850 | 110.188 |
| run-view | 5 | 145.659 | 141.429 | 167.572 | 136.478 | 167.572 |


<!-- trace-bench:8638a764ccddc3db3c8f3bf0bcea688bdd02ddcf -->
## 2026-04-09 11:23:56 UTC

- PR: [#1189](https://github.com/pingcap/agent-git-service/pull/1189) feat: add a user kind for respionse
- PR resolution: resolved
- Author: @Icemap
- PR merged at: 2026-04-09T11:22:04Z
- Merge commit: `8638a764ccddc3db3c8f3bf0bcea688bdd02ddcf`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24187514367)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 45.130 | 45.282 | 46.261 | 43.562 | 46.261 |
| auth-status | 5 | 47.026 | 46.680 | 49.561 | 45.227 | 49.561 |
| auth-logout | 5 | 37.171 | 37.004 | 38.536 | 35.653 | 38.536 |
| repo-create | 5 | 55.227 | 55.232 | 56.427 | 53.691 | 56.427 |
| repo-view | 5 | 79.741 | 80.977 | 83.435 | 74.420 | 83.435 |
| repo-clone | 5 | 143.875 | 135.131 | 167.033 | 132.873 | 167.033 |
| issue-create | 5 | 129.257 | 128.777 | 132.263 | 127.021 | 132.263 |
| issue-list | 5 | 57.004 | 57.149 | 58.956 | 55.100 | 58.956 |
| issue-view | 5 | 74.907 | 74.328 | 78.093 | 72.683 | 78.093 |
| pr-create | 5 | 226.590 | 226.143 | 231.017 | 223.367 | 231.017 |
| pr-list | 5 | 67.387 | 67.962 | 70.726 | 63.980 | 70.726 |
| pr-view | 5 | 118.022 | 116.347 | 125.182 | 114.307 | 125.182 |
| pr-merge | 5 | 118.778 | 118.100 | 124.073 | 115.420 | 124.073 |
| workflow-list | 5 | 52.729 | 53.314 | 55.258 | 49.102 | 55.258 |
| workflow-run | 5 | 88.504 | 87.526 | 91.908 | 85.065 | 91.908 |
| run-view | 5 | 125.801 | 118.610 | 154.182 | 116.811 | 154.182 |


<!-- trace-bench:2a813e5c30fd916f85f15af00c33f18d2782712b -->
## 2026-04-09 16:57:07 UTC

- PR: [#1190](https://github.com/pingcap/agent-git-service/pull/1190) fix: fall back to issue body for conversation titles
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-09T16:55:04Z
- Merge commit: `2a813e5c30fd916f85f15af00c33f18d2782712b`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24202578629)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 44.484 | 44.154 | 45.971 | 43.700 | 45.971 |
| auth-status | 5 | 45.862 | 45.893 | 46.173 | 45.256 | 46.173 |
| auth-logout | 5 | 37.440 | 37.059 | 40.026 | 34.361 | 40.026 |
| repo-create | 5 | 54.486 | 54.297 | 56.677 | 51.293 | 56.677 |
| repo-view | 5 | 73.428 | 72.879 | 76.788 | 71.220 | 76.788 |
| repo-clone | 5 | 133.094 | 134.958 | 135.475 | 128.484 | 135.475 |
| issue-create | 5 | 127.132 | 127.425 | 131.190 | 123.858 | 131.190 |
| issue-list | 5 | 56.260 | 55.036 | 60.056 | 53.429 | 60.056 |
| issue-view | 5 | 74.396 | 73.670 | 77.880 | 72.277 | 77.880 |
| pr-create | 5 | 231.807 | 225.413 | 260.378 | 218.300 | 260.378 |
| pr-list | 5 | 69.425 | 68.299 | 72.908 | 67.155 | 72.908 |
| pr-view | 5 | 118.357 | 118.832 | 120.830 | 116.015 | 120.830 |
| pr-merge | 5 | 123.413 | 117.348 | 149.385 | 115.869 | 149.385 |
| workflow-list | 5 | 52.305 | 52.256 | 53.363 | 51.416 | 53.363 |
| workflow-run | 5 | 93.477 | 88.758 | 119.129 | 83.624 | 119.129 |
| run-view | 5 | 116.581 | 116.294 | 120.377 | 114.474 | 120.377 |


<!-- trace-bench:2c33d331972a599e374ed1272000e374d88bd6e7 -->
## 2026-04-10 08:07:00 UTC

- PR: [#1193](https://github.com/pingcap/agent-git-service/pull/1193) fix: move trace bench history to dedicated repo
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-10T08:04:57Z
- Merge commit: `2c33d331972a599e374ed1272000e374d88bd6e7`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24233114588)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 41.700 | 40.964 | 44.868 | 38.637 | 44.868 |
| auth-status | 5 | 41.303 | 41.635 | 43.791 | 39.476 | 43.791 |
| auth-logout | 5 | 35.921 | 35.469 | 39.621 | 34.181 | 39.621 |
| repo-create | 5 | 53.434 | 52.894 | 57.919 | 50.459 | 57.919 |
| repo-view | 5 | 82.113 | 77.106 | 108.878 | 72.327 | 108.878 |
| repo-clone | 5 | 131.172 | 131.809 | 132.484 | 129.582 | 132.484 |
| issue-create | 5 | 123.372 | 123.278 | 124.364 | 122.718 | 124.364 |
| issue-list | 5 | 57.474 | 58.871 | 60.707 | 53.274 | 60.707 |
| issue-view | 5 | 72.480 | 71.685 | 74.585 | 71.326 | 74.585 |
| pr-create | 5 | 215.404 | 213.735 | 219.195 | 212.136 | 219.195 |
| pr-list | 5 | 64.694 | 64.400 | 67.344 | 63.204 | 67.344 |
| pr-view | 5 | 113.318 | 113.268 | 114.102 | 112.525 | 114.102 |
| pr-merge | 5 | 113.341 | 112.989 | 115.858 | 111.939 | 115.858 |
| workflow-list | 5 | 48.520 | 48.432 | 50.646 | 46.917 | 50.646 |
| workflow-run | 5 | 87.019 | 82.237 | 111.134 | 79.081 | 111.134 |
| run-view | 5 | 112.227 | 112.519 | 114.671 | 109.055 | 114.671 |


<!-- trace-bench:8a47d281b4ee07dda6295a4586f4ce6834957356 -->
## 2026-04-10 20:35:52 UTC

- PR: [#1194](https://github.com/pingcap/agent-git-service/pull/1194) fix: preserve collaborator created_at on update
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-10T20:33:48Z
- Merge commit: `8a47d281b4ee07dda6295a4586f4ce6834957356`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24262938740)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 55.686 | 55.240 | 59.263 | 54.200 | 59.263 |
| auth-status | 5 | 56.366 | 55.867 | 59.728 | 54.337 | 59.728 |
| auth-logout | 5 | 41.883 | 42.993 | 43.566 | 38.848 | 43.566 |
| repo-create | 5 | 68.641 | 67.638 | 77.385 | 62.294 | 77.385 |
| repo-view | 5 | 97.403 | 98.687 | 101.400 | 93.155 | 101.400 |
| repo-clone | 5 | 173.296 | 166.188 | 194.457 | 162.540 | 194.457 |
| issue-create | 5 | 155.786 | 158.023 | 159.018 | 151.243 | 159.018 |
| issue-list | 5 | 67.144 | 67.556 | 69.326 | 63.110 | 69.326 |
| issue-view | 5 | 90.696 | 90.778 | 94.147 | 88.138 | 94.147 |
| pr-create | 5 | 278.852 | 279.466 | 285.956 | 272.912 | 285.956 |
| pr-list | 5 | 77.229 | 78.988 | 81.917 | 72.286 | 81.917 |
| pr-view | 5 | 158.550 | 151.015 | 182.676 | 145.329 | 182.676 |
| pr-merge | 5 | 149.224 | 148.081 | 154.283 | 145.482 | 154.283 |
| workflow-list | 5 | 56.609 | 57.493 | 58.780 | 54.349 | 58.780 |
| workflow-run | 5 | 107.113 | 106.910 | 110.808 | 104.087 | 110.808 |
| run-view | 5 | 150.108 | 147.154 | 169.358 | 140.472 | 169.358 |


<!-- trace-bench:6d0565bd07fff9748c74d6e56cca6ffcdd64d97a -->
## 2026-04-11 09:36:58 UTC

- PR: [#1195](https://github.com/pingcap/agent-git-service/pull/1195) build(deps-dev): bump basic-ftp from 5.2.1 to 5.2.2 in /web
- PR resolution: resolved
- Author: @dependabot[bot]
- PR merged at: 2026-04-11T09:34:50Z
- Merge commit: `6d0565bd07fff9748c74d6e56cca6ffcdd64d97a`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24279705159)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 46.664 | 46.992 | 48.700 | 44.647 | 48.700 |
| auth-status | 5 | 46.273 | 45.473 | 49.379 | 44.277 | 49.379 |
| auth-logout | 5 | 37.306 | 37.416 | 37.681 | 36.548 | 37.681 |
| repo-create | 5 | 57.429 | 56.695 | 60.556 | 55.344 | 60.556 |
| repo-view | 5 | 81.338 | 80.508 | 87.819 | 76.418 | 87.819 |
| repo-clone | 5 | 153.687 | 145.954 | 176.891 | 145.021 | 176.891 |
| issue-create | 5 | 132.026 | 131.069 | 135.107 | 130.157 | 135.107 |
| issue-list | 5 | 59.630 | 60.072 | 61.172 | 57.705 | 61.172 |
| issue-view | 5 | 76.868 | 75.478 | 80.572 | 73.048 | 80.572 |
| pr-create | 5 | 225.719 | 223.947 | 230.158 | 222.801 | 230.158 |
| pr-list | 5 | 66.310 | 65.703 | 68.753 | 64.890 | 68.753 |
| pr-view | 5 | 116.899 | 117.892 | 118.863 | 112.248 | 118.863 |
| pr-merge | 5 | 117.090 | 117.857 | 119.119 | 115.079 | 119.119 |
| workflow-list | 5 | 51.599 | 51.180 | 54.974 | 48.842 | 54.974 |
| workflow-run | 5 | 85.180 | 86.433 | 87.014 | 81.276 | 87.014 |
| run-view | 5 | 124.262 | 118.945 | 147.604 | 115.707 | 147.604 |


<!-- trace-bench:bd4af900cc3b112d602c71b78dfc1675ca061334 -->
## 2026-04-12 14:16:45 UTC

- PR: [#1197](https://github.com/pingcap/agent-git-service/pull/1197) fix: align org invitation roles with GitHub semantics
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-12T14:14:40Z
- Merge commit: `bd4af900cc3b112d602c71b78dfc1675ca061334`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24308682366)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 54.731 | 53.784 | 58.361 | 52.330 | 58.361 |
| auth-status | 5 | 53.139 | 52.853 | 54.978 | 51.778 | 54.978 |
| auth-logout | 5 | 43.233 | 43.282 | 44.871 | 41.432 | 44.871 |
| repo-create | 5 | 65.254 | 64.740 | 70.102 | 62.699 | 70.102 |
| repo-view | 5 | 97.451 | 97.509 | 101.371 | 94.488 | 101.371 |
| repo-clone | 5 | 173.598 | 170.189 | 197.179 | 159.023 | 197.179 |
| issue-create | 5 | 153.164 | 153.554 | 156.947 | 148.816 | 156.947 |
| issue-list | 5 | 63.401 | 63.488 | 64.544 | 62.558 | 64.544 |
| issue-view | 5 | 85.320 | 85.642 | 87.862 | 81.955 | 87.862 |
| pr-create | 5 | 280.417 | 270.379 | 306.682 | 267.494 | 306.682 |
| pr-list | 5 | 83.256 | 76.540 | 114.187 | 73.874 | 114.187 |
| pr-view | 5 | 142.963 | 141.826 | 152.533 | 137.476 | 152.533 |
| pr-merge | 5 | 153.366 | 151.393 | 176.003 | 142.145 | 176.003 |
| workflow-list | 5 | 55.689 | 56.178 | 56.408 | 54.746 | 56.408 |
| workflow-run | 5 | 100.341 | 100.301 | 105.244 | 97.424 | 105.244 |
| run-view | 5 | 138.741 | 135.123 | 157.609 | 129.165 | 157.609 |


<!-- trace-bench:700a1c76516b6c4b6fa6a5a2ec9f8a01bb0764d7 -->
## 2026-04-12 15:15:37 UTC

- PR: [#1198](https://github.com/pingcap/agent-git-service/pull/1198) chore: remove web frontend and clean stale references
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-12T15:13:20Z
- Merge commit: `700a1c76516b6c4b6fa6a5a2ec9f8a01bb0764d7`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24309751841)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 52.544 | 53.085 | 54.111 | 50.822 | 54.111 |
| auth-status | 5 | 53.803 | 53.414 | 56.365 | 51.694 | 56.365 |
| auth-logout | 5 | 43.429 | 42.787 | 46.902 | 41.629 | 46.902 |
| repo-create | 5 | 64.565 | 63.402 | 70.201 | 61.698 | 70.201 |
| repo-view | 5 | 96.497 | 91.803 | 111.832 | 89.585 | 111.832 |
| repo-clone | 5 | 167.658 | 165.872 | 178.923 | 160.420 | 178.923 |
| issue-create | 5 | 148.191 | 145.559 | 154.890 | 141.252 | 154.890 |
| issue-list | 5 | 68.419 | 67.162 | 75.773 | 64.280 | 75.773 |
| issue-view | 5 | 90.925 | 89.875 | 96.191 | 85.796 | 96.191 |
| pr-create | 5 | 258.801 | 258.883 | 266.951 | 249.500 | 266.951 |
| pr-list | 5 | 72.762 | 72.766 | 74.556 | 70.070 | 74.556 |
| pr-view | 5 | 143.170 | 136.995 | 171.194 | 131.400 | 171.194 |
| pr-merge | 5 | 142.898 | 143.052 | 145.553 | 140.494 | 145.553 |
| workflow-list | 5 | 54.175 | 54.397 | 55.384 | 52.920 | 55.384 |
| workflow-run | 5 | 98.037 | 99.008 | 102.399 | 94.038 | 102.399 |
| run-view | 5 | 136.783 | 128.693 | 159.517 | 127.870 | 159.517 |


<!-- trace-bench:7baed76c5a637a93e45ac9fb6772ba832c6b421d -->
## 2026-04-12 17:15:30 UTC

- PR: [#1199](https://github.com/pingcap/agent-git-service/pull/1199) feat: add PUT org membership role updates
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-12T17:13:11Z
- Merge commit: `7baed76c5a637a93e45ac9fb6772ba832c6b421d`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24312002343)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 45.387 | 45.534 | 46.241 | 44.536 | 46.241 |
| auth-status | 5 | 47.577 | 46.419 | 51.417 | 46.196 | 51.417 |
| auth-logout | 5 | 35.898 | 35.394 | 38.000 | 34.165 | 38.000 |
| repo-create | 5 | 59.632 | 60.149 | 61.722 | 56.697 | 61.722 |
| repo-view | 5 | 84.194 | 85.731 | 87.967 | 78.027 | 87.967 |
| repo-clone | 5 | 158.580 | 150.013 | 192.870 | 148.562 | 192.870 |
| issue-create | 5 | 145.751 | 142.773 | 159.066 | 141.074 | 159.066 |
| issue-list | 5 | 61.111 | 60.743 | 62.941 | 59.598 | 62.941 |
| issue-view | 5 | 84.276 | 83.929 | 86.914 | 83.219 | 86.914 |
| pr-create | 5 | 271.581 | 271.202 | 280.497 | 260.705 | 280.497 |
| pr-list | 5 | 77.537 | 77.695 | 79.840 | 75.516 | 79.840 |
| pr-view | 5 | 145.069 | 138.714 | 175.408 | 135.019 | 175.408 |
| pr-merge | 5 | 143.678 | 143.501 | 144.851 | 142.799 | 144.851 |
| workflow-list | 5 | 53.345 | 52.587 | 55.271 | 51.529 | 55.271 |
| workflow-run | 5 | 98.975 | 97.805 | 105.718 | 95.550 | 105.718 |
| run-view | 5 | 138.207 | 131.210 | 166.528 | 124.487 | 166.528 |


<!-- trace-bench:ddcf7c107da9bdce00516bfc63f6dab0daf7ed05 -->
## 2026-04-13 07:00:26 UTC

- PR: [#1200](https://github.com/pingcap/agent-git-service/pull/1200) fix: align team membership semantics with GitHub
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-13T06:58:24Z
- Merge commit: `ddcf7c107da9bdce00516bfc63f6dab0daf7ed05`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24330045835)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.182 | 51.762 | 54.010 | 47.493 | 54.010 |
| auth-status | 5 | 52.492 | 51.413 | 56.867 | 49.281 | 56.867 |
| auth-logout | 5 | 40.970 | 39.404 | 46.509 | 39.002 | 46.509 |
| repo-create | 5 | 62.519 | 60.607 | 67.919 | 59.382 | 67.919 |
| repo-view | 5 | 90.586 | 91.608 | 94.935 | 84.870 | 94.935 |
| repo-clone | 5 | 171.033 | 164.442 | 201.212 | 156.283 | 201.212 |
| issue-create | 5 | 159.477 | 159.719 | 163.032 | 153.377 | 163.032 |
| issue-list | 5 | 69.027 | 68.881 | 71.352 | 67.592 | 71.352 |
| issue-view | 5 | 93.062 | 93.955 | 95.970 | 89.846 | 95.970 |
| pr-create | 5 | 280.058 | 279.113 | 291.114 | 269.513 | 291.114 |
| pr-list | 5 | 76.012 | 74.548 | 84.070 | 71.976 | 84.070 |
| pr-view | 5 | 149.671 | 144.532 | 175.668 | 136.245 | 175.668 |
| pr-merge | 5 | 144.804 | 144.406 | 147.908 | 143.293 | 147.908 |
| workflow-list | 5 | 100.811 | 56.700 | 266.083 | 53.782 | 266.083 |
| workflow-run | 5 | 132.067 | 103.597 | 242.274 | 100.439 | 242.274 |
| run-view | 5 | 147.149 | 144.453 | 164.868 | 135.397 | 164.868 |


<!-- trace-bench:1a089168847c27c0ec0c5ae6ec06deb5fcf3bf85 -->
## 2026-04-13 07:56:54 UTC

- PR: [#1201](https://github.com/pingcap/agent-git-service/pull/1201) Add .test to .gitignore
- PR resolution: resolved
- Author: @IANTHEREAL
- PR merged at: 2026-04-13T07:54:48Z
- Merge commit: `1a089168847c27c0ec0c5ae6ec06deb5fcf3bf85`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24332158332)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 46.358 | 45.589 | 49.276 | 45.016 | 49.276 |
| auth-status | 5 | 47.870 | 47.010 | 52.896 | 45.933 | 52.896 |
| auth-logout | 5 | 37.035 | 36.988 | 38.175 | 36.058 | 38.175 |
| repo-create | 5 | 56.424 | 56.973 | 57.990 | 53.614 | 57.990 |
| repo-view | 5 | 81.392 | 80.838 | 86.647 | 77.283 | 86.647 |
| repo-clone | 5 | 150.654 | 142.568 | 174.372 | 141.635 | 174.372 |
| issue-create | 5 | 131.887 | 129.395 | 137.203 | 128.433 | 137.203 |
| issue-list | 5 | 57.956 | 58.054 | 59.706 | 56.838 | 59.706 |
| issue-view | 5 | 78.071 | 78.519 | 80.268 | 75.828 | 80.268 |
| pr-create | 5 | 238.018 | 232.374 | 262.039 | 224.627 | 262.039 |
| pr-list | 5 | 66.314 | 65.649 | 69.319 | 64.155 | 69.319 |
| pr-view | 5 | 128.602 | 123.590 | 153.883 | 117.565 | 153.883 |
| pr-merge | 5 | 119.585 | 119.527 | 127.570 | 114.899 | 127.570 |
| workflow-list | 5 | 50.875 | 51.259 | 52.403 | 48.656 | 52.403 |
| workflow-run | 5 | 87.333 | 86.933 | 91.475 | 84.010 | 91.475 |
| run-view | 5 | 126.583 | 120.434 | 155.073 | 117.028 | 155.073 |


<!-- trace-bench:705430419b3932e7d9aa66c4db24bf0ea8a30cec -->
## 2026-04-13 08:01:59 UTC

- PR: [#1202](https://github.com/pingcap/agent-git-service/pull/1202) fix: align team membership semantics and add pending invitations endpoint
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-13T07:59:43Z
- Merge commit: `705430419b3932e7d9aa66c4db24bf0ea8a30cec`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24332353721)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 49.465 | 49.372 | 52.215 | 47.500 | 52.215 |
| auth-status | 5 | 52.878 | 52.636 | 55.833 | 50.588 | 55.833 |
| auth-logout | 5 | 39.337 | 39.639 | 43.268 | 36.976 | 43.268 |
| repo-create | 5 | 63.887 | 63.165 | 66.108 | 61.485 | 66.108 |
| repo-view | 5 | 93.210 | 89.819 | 110.853 | 85.335 | 110.853 |
| repo-clone | 5 | 161.691 | 160.293 | 166.388 | 159.022 | 166.388 |
| issue-create | 5 | 157.307 | 158.063 | 159.456 | 153.380 | 159.456 |
| issue-list | 5 | 66.068 | 64.064 | 74.498 | 61.652 | 74.498 |
| issue-view | 5 | 90.029 | 86.348 | 104.099 | 83.586 | 104.099 |
| pr-create | 5 | 298.881 | 296.938 | 302.897 | 296.360 | 302.897 |
| pr-list | 5 | 87.510 | 87.882 | 90.502 | 84.994 | 90.502 |
| pr-view | 5 | 155.190 | 154.894 | 164.824 | 147.920 | 164.824 |
| pr-merge | 5 | 165.315 | 164.975 | 179.907 | 153.321 | 179.907 |
| workflow-list | 5 | 66.230 | 66.032 | 68.123 | 64.560 | 68.123 |
| workflow-run | 5 | 128.815 | 120.853 | 163.945 | 113.734 | 163.945 |
| run-view | 5 | 161.387 | 162.010 | 173.705 | 153.887 | 173.705 |


<!-- trace-bench:eab0719e6b063c5f350a84e6582b91dad586c17f -->
## 2026-04-13 15:20:05 UTC

- PR: [#1203](https://github.com/pingcap/agent-git-service/pull/1203) fix: narrow filtered semantic search ranking queries
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-13T15:17:51Z
- Merge commit: `eab0719e6b063c5f350a84e6582b91dad586c17f`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24351351596)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 59.505 | 58.832 | 67.852 | 54.952 | 67.852 |
| auth-status | 5 | 55.904 | 56.401 | 57.310 | 53.502 | 57.310 |
| auth-logout | 5 | 44.245 | 44.634 | 45.512 | 42.134 | 45.512 |
| repo-create | 5 | 65.957 | 65.521 | 69.168 | 64.086 | 69.168 |
| repo-view | 5 | 99.150 | 98.330 | 102.951 | 95.839 | 102.951 |
| repo-clone | 5 | 170.145 | 162.941 | 193.545 | 161.263 | 193.545 |
| issue-create | 5 | 150.827 | 149.561 | 158.076 | 145.520 | 158.076 |
| issue-list | 5 | 64.354 | 62.880 | 68.457 | 61.499 | 68.457 |
| issue-view | 5 | 89.546 | 88.781 | 95.175 | 85.192 | 95.175 |
| pr-create | 5 | 292.323 | 280.182 | 317.877 | 271.556 | 317.877 |
| pr-list | 5 | 75.106 | 75.184 | 76.495 | 72.786 | 76.495 |
| pr-view | 5 | 143.274 | 141.655 | 151.889 | 138.483 | 151.889 |
| pr-merge | 5 | 146.870 | 145.926 | 149.672 | 145.479 | 149.672 |
| workflow-list | 5 | 61.918 | 59.818 | 72.302 | 56.140 | 72.302 |
| workflow-run | 5 | 108.019 | 103.881 | 117.664 | 101.704 | 117.664 |
| run-view | 5 | 149.774 | 141.465 | 176.329 | 139.569 | 176.329 |


<!-- trace-bench:c60f0a0eb97d1bb5b8981aa185c9b1536a59e121 -->
## 2026-04-14 02:19:14 UTC

- PR: [#1204](https://github.com/pingcap/agent-git-service/pull/1204) build(deps): bump github.com/sigstore/timestamp-authority/v2 from 2.0.3 to 2.0.6 in /cli
- PR resolution: resolved
- Author: @dependabot[bot]
- PR merged at: 2026-04-14T02:16:00Z
- Merge commit: `c60f0a0eb97d1bb5b8981aa185c9b1536a59e121`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24377348901)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 47.633 | 47.464 | 48.665 | 46.779 | 48.665 |
| auth-status | 5 | 49.940 | 50.129 | 51.236 | 48.545 | 51.236 |
| auth-logout | 5 | 40.565 | 39.756 | 42.945 | 38.874 | 42.945 |
| repo-create | 5 | 58.167 | 58.104 | 60.680 | 55.062 | 60.680 |
| repo-view | 5 | 81.791 | 83.159 | 83.729 | 77.911 | 83.729 |
| repo-clone | 5 | 145.622 | 145.123 | 148.699 | 142.185 | 148.699 |
| issue-create | 5 | 133.508 | 130.909 | 142.377 | 128.525 | 142.377 |
| issue-list | 5 | 61.920 | 60.651 | 67.078 | 58.772 | 67.078 |
| issue-view | 5 | 78.655 | 78.428 | 81.315 | 77.010 | 81.315 |
| pr-create | 5 | 241.856 | 235.004 | 278.405 | 223.604 | 278.405 |
| pr-list | 5 | 69.787 | 69.789 | 70.908 | 68.840 | 70.908 |
| pr-view | 5 | 120.206 | 120.584 | 121.853 | 117.215 | 121.853 |
| pr-merge | 5 | 123.347 | 123.594 | 128.200 | 118.270 | 128.200 |
| workflow-list | 5 | 54.246 | 54.399 | 56.559 | 52.687 | 56.559 |
| workflow-run | 5 | 89.399 | 89.617 | 93.536 | 84.722 | 93.536 |
| run-view | 5 | 120.643 | 119.540 | 126.451 | 117.464 | 126.451 |


<!-- trace-bench:c71c1dcee2a10b43dc76ea617d083e89799feceb -->
## 2026-04-16 11:24:06 UTC

- PR: [#1205](https://github.com/pingcap/agent-git-service/pull/1205) perf: eliminate redundant preloading in Create PR (#1079)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-16T11:22:01Z
- Merge commit: `c71c1dcee2a10b43dc76ea617d083e89799feceb`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24507449278)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 47.203 | 47.480 | 48.529 | 45.914 | 48.529 |
| auth-status | 5 | 49.963 | 48.885 | 55.279 | 48.036 | 55.279 |
| auth-logout | 5 | 38.045 | 38.003 | 38.389 | 37.818 | 38.389 |
| repo-create | 5 | 59.059 | 57.774 | 65.540 | 56.167 | 65.540 |
| repo-view | 5 | 82.906 | 82.172 | 88.870 | 77.485 | 88.870 |
| repo-clone | 5 | 149.421 | 140.857 | 182.507 | 139.535 | 182.507 |
| issue-create | 5 | 137.078 | 135.097 | 142.228 | 133.063 | 142.228 |
| issue-list | 5 | 58.410 | 57.638 | 60.736 | 57.321 | 60.736 |
| issue-view | 5 | 81.263 | 80.443 | 84.022 | 78.968 | 84.022 |
| pr-create | 5 | 223.296 | 214.413 | 247.144 | 213.194 | 247.144 |
| pr-list | 5 | 76.577 | 69.801 | 107.056 | 67.181 | 107.056 |
| pr-view | 5 | 128.786 | 122.895 | 155.541 | 119.143 | 155.541 |
| pr-merge | 5 | 120.533 | 120.558 | 122.810 | 116.165 | 122.810 |
| workflow-list | 5 | 52.716 | 52.141 | 56.604 | 50.211 | 56.604 |
| workflow-run | 5 | 89.382 | 88.970 | 90.468 | 88.550 | 90.468 |
| run-view | 5 | 123.675 | 124.729 | 126.934 | 118.804 | 126.934 |


<!-- trace-bench:eaa580e30659124bb2671b75f767e530c6fe52ad -->
## 2026-04-16 12:09:37 UTC

- PR: [#1206](https://github.com/pingcap/agent-git-service/pull/1206) perf: merge LIKE + Vector search results before preloading (#1077)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-16T12:07:19Z
- Merge commit: `eaa580e30659124bb2671b75f767e530c6fe52ad`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24509295416)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.984 | 51.935 | 52.837 | 51.495 | 52.837 |
| auth-status | 5 | 54.439 | 54.061 | 56.614 | 53.365 | 56.614 |
| auth-logout | 5 | 41.999 | 42.478 | 43.192 | 40.492 | 43.192 |
| repo-create | 5 | 66.800 | 67.243 | 70.522 | 63.464 | 70.522 |
| repo-view | 5 | 97.150 | 96.967 | 99.489 | 94.630 | 99.489 |
| repo-clone | 5 | 173.247 | 172.771 | 198.693 | 155.284 | 198.693 |
| issue-create | 5 | 161.933 | 155.540 | 181.606 | 151.283 | 181.606 |
| issue-list | 5 | 65.796 | 65.641 | 72.215 | 61.652 | 72.215 |
| issue-view | 5 | 87.683 | 87.868 | 90.940 | 85.249 | 90.940 |
| pr-create | 5 | 260.246 | 254.725 | 287.207 | 246.243 | 287.207 |
| pr-list | 5 | 87.402 | 82.756 | 110.515 | 78.897 | 110.515 |
| pr-view | 5 | 143.395 | 141.274 | 151.330 | 137.954 | 151.330 |
| pr-merge | 5 | 147.672 | 142.580 | 166.547 | 141.400 | 166.547 |
| workflow-list | 5 | 55.209 | 54.915 | 58.959 | 52.380 | 58.959 |
| workflow-run | 5 | 104.682 | 100.912 | 126.344 | 93.312 | 126.344 |
| run-view | 5 | 136.115 | 135.424 | 144.041 | 125.736 | 144.041 |

