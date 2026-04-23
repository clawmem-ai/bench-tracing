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


<!-- trace-bench:128076b11a9a3646d2ecec26e022673877a597db -->
## 2026-04-16 20:08:24 UTC

- PR: [#1207](https://github.com/pingcap/agent-git-service/pull/1207) Implement P1: End-to-end multi-agent/multi-tenant isolation
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-16T20:06:11Z
- Merge commit: `128076b11a9a3646d2ecec26e022673877a597db`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24531391791)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 50.558 | 49.768 | 52.803 | 48.989 | 52.803 |
| auth-status | 5 | 52.772 | 53.727 | 54.632 | 50.025 | 54.632 |
| auth-logout | 5 | 41.043 | 40.733 | 43.371 | 39.087 | 43.371 |
| repo-create | 5 | 66.483 | 65.944 | 69.417 | 63.469 | 69.417 |
| repo-view | 5 | 110.446 | 99.877 | 158.713 | 94.568 | 158.713 |
| repo-clone | 5 | 174.978 | 175.116 | 179.323 | 171.440 | 179.323 |
| issue-create | 5 | 170.077 | 172.070 | 173.909 | 159.922 | 173.909 |
| issue-list | 5 | 69.992 | 68.574 | 77.788 | 64.140 | 77.788 |
| issue-view | 5 | 91.336 | 92.323 | 93.396 | 86.313 | 93.396 |
| pr-create | 5 | 281.854 | 290.183 | 292.474 | 249.963 | 292.474 |
| pr-list | 5 | 84.237 | 84.682 | 86.552 | 82.067 | 86.552 |
| pr-view | 5 | 140.177 | 139.580 | 142.619 | 138.289 | 142.619 |
| pr-merge | 5 | 152.563 | 145.711 | 182.269 | 142.628 | 182.269 |
| workflow-list | 5 | 59.051 | 58.906 | 62.972 | 54.885 | 62.972 |
| workflow-run | 5 | 190.709 | 106.991 | 527.673 | 102.964 | 527.673 |
| run-view | 5 | 129.920 | 129.193 | 139.814 | 122.282 | 139.814 |


<!-- trace-bench:f6a5fb28b93b173e6b745d4cfdcefe84fb2b66c1 -->
## 2026-04-16 23:27:50 UTC

- PR: [#1208](https://github.com/pingcap/agent-git-service/pull/1208) build(deps): bump github.com/jackc/pgx/v5 from 5.6.0 to 5.9.0
- PR resolution: resolved
- Author: @dependabot[bot]
- PR merged at: 2026-04-16T23:24:22Z
- Merge commit: `f6a5fb28b93b173e6b745d4cfdcefe84fb2b66c1`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24539214011)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.130 | 47.664 | 63.011 | 45.219 | 63.011 |
| auth-status | 5 | 48.689 | 47.954 | 50.661 | 47.569 | 50.661 |
| auth-logout | 5 | 36.885 | 36.717 | 38.350 | 35.682 | 38.350 |
| repo-create | 5 | 59.714 | 59.524 | 61.982 | 58.024 | 61.982 |
| repo-view | 5 | 91.561 | 86.954 | 113.079 | 84.135 | 113.079 |
| repo-clone | 5 | 163.023 | 157.507 | 185.716 | 156.909 | 185.716 |
| issue-create | 5 | 151.104 | 149.478 | 159.617 | 147.076 | 159.617 |
| issue-list | 5 | 65.314 | 65.608 | 66.377 | 63.672 | 66.377 |
| issue-view | 5 | 85.455 | 86.301 | 88.501 | 80.851 | 88.501 |
| pr-create | 5 | 255.819 | 248.673 | 281.328 | 247.314 | 281.328 |
| pr-list | 5 | 83.417 | 75.643 | 112.019 | 74.426 | 112.019 |
| pr-view | 5 | 144.744 | 140.746 | 164.042 | 137.970 | 164.042 |
| pr-merge | 5 | 144.063 | 144.282 | 145.064 | 142.984 | 145.064 |
| workflow-list | 5 | 57.145 | 56.378 | 63.424 | 54.137 | 63.424 |
| workflow-run | 5 | 100.144 | 101.068 | 103.087 | 94.820 | 103.087 |
| run-view | 5 | 135.599 | 135.364 | 140.462 | 131.167 | 140.462 |


<!-- trace-bench:d7dc073620c7e3146590da1e7881df9fb1a72865 -->
## 2026-04-18 01:44:11 UTC

- PR: [#1209](https://github.com/pingcap/agent-git-service/pull/1209) build(deps): bump github.com/go-git/go-git/v5 from 5.17.1 to 5.18.0
- PR resolution: resolved
- Author: @dependabot[bot]
- PR merged at: 2026-04-18T01:40:44Z
- Merge commit: `d7dc073620c7e3146590da1e7881df9fb1a72865`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24594030470)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 47.132 | 46.797 | 49.072 | 46.096 | 49.072 |
| auth-status | 5 | 48.362 | 48.182 | 49.836 | 47.067 | 49.836 |
| auth-logout | 5 | 37.746 | 37.934 | 38.737 | 36.368 | 38.737 |
| repo-create | 5 | 60.506 | 58.877 | 67.092 | 58.117 | 67.092 |
| repo-view | 5 | 84.615 | 84.349 | 86.442 | 83.446 | 86.442 |
| repo-clone | 5 | 165.572 | 162.149 | 185.523 | 153.870 | 185.523 |
| issue-create | 5 | 153.102 | 152.594 | 154.594 | 151.557 | 154.594 |
| issue-list | 5 | 62.905 | 62.269 | 65.436 | 60.553 | 65.436 |
| issue-view | 5 | 85.085 | 86.331 | 86.953 | 81.515 | 86.953 |
| pr-create | 5 | 255.048 | 253.587 | 268.417 | 247.169 | 268.417 |
| pr-list | 5 | 76.254 | 75.795 | 78.890 | 73.851 | 78.890 |
| pr-view | 5 | 141.330 | 141.113 | 147.568 | 136.906 | 147.568 |
| pr-merge | 5 | 145.606 | 144.453 | 149.584 | 143.454 | 149.584 |
| workflow-list | 5 | 55.177 | 55.336 | 55.411 | 54.584 | 55.411 |
| workflow-run | 5 | 101.798 | 100.585 | 107.031 | 98.633 | 107.031 |
| run-view | 5 | 142.565 | 138.541 | 163.814 | 131.802 | 163.814 |


<!-- trace-bench:1edf061cd2201aa61deccf9ea023f643822d256d -->
## 2026-04-21 08:40:07 UTC

- PR: [#1210](https://github.com/pingcap/agent-git-service/pull/1210) chore: track console and clawmem plugins as submodules
- PR resolution: resolved
- Author: @Icemap
- PR merged at: 2026-04-21T08:38:10Z
- Merge commit: `1edf061cd2201aa61deccf9ea023f643822d256d`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24712653909)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 52.499 | 52.607 | 53.122 | 51.678 | 53.122 |
| auth-status | 5 | 53.798 | 52.788 | 57.150 | 52.366 | 57.150 |
| auth-logout | 5 | 41.995 | 42.169 | 42.917 | 41.240 | 42.917 |
| repo-create | 5 | 66.497 | 66.693 | 72.446 | 63.242 | 72.446 |
| repo-view | 5 | 92.433 | 91.848 | 94.708 | 91.541 | 94.708 |
| repo-clone | 5 | 180.748 | 176.359 | 203.568 | 167.639 | 203.568 |
| issue-create | 5 | 158.523 | 157.560 | 166.992 | 152.886 | 166.992 |
| issue-list | 5 | 70.318 | 70.140 | 74.551 | 66.746 | 74.551 |
| issue-view | 5 | 92.489 | 92.249 | 93.214 | 91.694 | 93.214 |
| pr-create | 5 | 271.540 | 262.183 | 319.283 | 251.109 | 319.283 |
| pr-list | 5 | 89.171 | 83.361 | 114.093 | 79.634 | 114.093 |
| pr-view | 5 | 146.543 | 143.970 | 157.347 | 141.841 | 157.347 |
| pr-merge | 5 | 144.354 | 144.738 | 153.214 | 138.043 | 153.214 |
| workflow-list | 5 | 57.196 | 56.867 | 59.792 | 54.284 | 59.792 |
| workflow-run | 5 | 118.438 | 113.821 | 148.783 | 106.074 | 148.783 |
| run-view | 5 | 137.611 | 137.923 | 144.314 | 132.829 | 144.314 |


<!-- trace-bench:146951cf0f59c881a0cc7472fb4455843a10ffbd -->
## 2026-04-21 08:50:51 UTC

- PR: [#1213](https://github.com/pingcap/agent-git-service/pull/1213) docs(clawmem-cc-plugin): drop finalize pipeline from revision plan
- PR resolution: resolved
- Author: @Icemap
- PR merged at: 2026-04-21T08:48:45Z
- Merge commit: `146951cf0f59c881a0cc7472fb4455843a10ffbd`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24713100797)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 55.157 | 56.281 | 57.138 | 52.362 | 57.138 |
| auth-status | 5 | 56.269 | 56.354 | 58.838 | 53.097 | 58.838 |
| auth-logout | 5 | 44.284 | 44.079 | 45.757 | 42.819 | 45.757 |
| repo-create | 5 | 72.057 | 72.353 | 74.565 | 68.642 | 74.565 |
| repo-view | 5 | 110.879 | 109.040 | 123.189 | 103.241 | 123.189 |
| repo-clone | 5 | 195.362 | 190.358 | 224.716 | 178.784 | 224.716 |
| issue-create | 5 | 176.421 | 177.038 | 179.109 | 170.832 | 179.109 |
| issue-list | 5 | 77.172 | 75.233 | 85.479 | 74.433 | 85.479 |
| issue-view | 5 | 102.017 | 105.656 | 110.238 | 92.756 | 110.238 |
| pr-create | 5 | 313.817 | 304.034 | 354.341 | 296.637 | 354.341 |
| pr-list | 5 | 98.755 | 94.293 | 114.544 | 90.811 | 114.544 |
| pr-view | 5 | 174.409 | 174.397 | 177.939 | 168.986 | 177.939 |
| pr-merge | 5 | 187.451 | 173.729 | 249.448 | 166.092 | 249.448 |
| workflow-list | 5 | 69.685 | 70.540 | 70.640 | 67.141 | 70.640 |
| workflow-run | 5 | 128.013 | 121.175 | 154.996 | 115.462 | 154.996 |
| run-view | 5 | 166.679 | 165.173 | 178.669 | 158.631 | 178.669 |


<!-- trace-bench:7f0cb00e743d17bfa844a8a84ac347d16b38aa57 -->
## 2026-04-21 15:55:39 UTC

- PR: [#1215](https://github.com/pingcap/agent-git-service/pull/1215) chore: track clawmem-codex-plugin as submodule
- PR resolution: resolved
- Author: @Icemap
- PR merged at: 2026-04-21T15:53:45Z
- Merge commit: `7f0cb00e743d17bfa844a8a84ac347d16b38aa57`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24732389505)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 81.558 | 81.320 | 95.377 | 71.414 | 95.377 |
| auth-status | 5 | 81.065 | 81.989 | 84.102 | 76.409 | 84.102 |
| auth-logout | 5 | 63.723 | 62.676 | 70.270 | 56.180 | 70.270 |
| repo-create | 5 | 99.215 | 100.230 | 103.383 | 92.572 | 103.383 |
| repo-view | 5 | 147.641 | 146.512 | 154.598 | 139.868 | 154.598 |
| repo-clone | 5 | 253.906 | 254.171 | 266.085 | 243.625 | 266.085 |
| issue-create | 5 | 155.626 | 153.791 | 160.328 | 152.066 | 160.328 |
| issue-list | 5 | 67.067 | 65.673 | 71.039 | 64.459 | 71.039 |
| issue-view | 5 | 92.144 | 91.434 | 96.829 | 89.554 | 96.829 |
| pr-create | 5 | 257.195 | 255.991 | 261.419 | 253.446 | 261.419 |
| pr-list | 5 | 81.279 | 81.756 | 82.243 | 79.395 | 82.243 |
| pr-view | 5 | 146.955 | 147.512 | 149.833 | 143.977 | 149.833 |
| pr-merge | 5 | 242.140 | 148.364 | 613.445 | 145.994 | 613.445 |
| workflow-list | 5 | 63.115 | 62.183 | 66.097 | 60.395 | 66.097 |
| workflow-run | 5 | 106.919 | 105.130 | 112.858 | 103.706 | 112.858 |
| run-view | 5 | 148.016 | 143.224 | 174.489 | 137.802 | 174.489 |


<!-- trace-bench:04d9fc30893685d6d143f67efbf30fb9570d513f -->
## 2026-04-21 23:49:39 UTC

- PR: [#1216](https://github.com/pingcap/agent-git-service/pull/1216) fix: security & correctness sweep from high→low audit (7 commits)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-21T23:47:23Z
- Merge commit: `04d9fc30893685d6d143f67efbf30fb9570d513f`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24752405596)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.682 | 51.252 | 53.918 | 50.461 | 53.918 |
| auth-status | 5 | 53.260 | 53.392 | 55.543 | 51.308 | 55.543 |
| auth-logout | 5 | 42.997 | 42.691 | 44.401 | 41.641 | 44.401 |
| repo-create | 5 | 64.824 | 64.323 | 68.779 | 61.483 | 68.779 |
| repo-view | 5 | 97.520 | 99.326 | 99.942 | 91.337 | 99.942 |
| repo-clone | 5 | 171.544 | 165.148 | 191.302 | 164.909 | 191.302 |
| issue-create | 5 | 153.180 | 152.286 | 160.671 | 149.014 | 160.671 |
| issue-list | 5 | 66.900 | 66.338 | 70.982 | 63.780 | 70.982 |
| issue-view | 5 | 89.643 | 89.306 | 95.843 | 86.593 | 95.843 |
| pr-create | 5 | 256.518 | 246.871 | 292.223 | 242.753 | 292.223 |
| pr-list | 5 | 88.092 | 84.378 | 111.970 | 78.157 | 111.970 |
| pr-view | 5 | 144.155 | 144.119 | 147.735 | 139.402 | 147.735 |
| pr-merge | 5 | 352.493 | 152.887 | 1134.200 | 146.290 | 1134.200 |
| workflow-list | 5 | 61.637 | 61.308 | 65.070 | 59.398 | 65.070 |
| workflow-run | 5 | 108.392 | 104.122 | 129.404 | 98.287 | 129.404 |
| run-view | 5 | 141.021 | 141.752 | 147.171 | 134.148 | 147.171 |


<!-- trace-bench:44004dfa9a6368412a1e6897a8984b1041a34913 -->
## 2026-04-22 01:47:03 UTC

- PR: [#1224](https://github.com/pingcap/agent-git-service/pull/1224) refactor: structural cleanup sweep (6 commits)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T01:44:45Z
- Merge commit: `44004dfa9a6368412a1e6897a8984b1041a34913`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24755836376)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 53.796 | 52.997 | 58.472 | 51.048 | 58.472 |
| auth-status | 5 | 53.547 | 53.517 | 56.399 | 51.566 | 56.399 |
| auth-logout | 5 | 44.257 | 43.196 | 49.004 | 42.847 | 49.004 |
| repo-create | 5 | 66.617 | 66.510 | 68.149 | 65.475 | 68.149 |
| repo-view | 5 | 99.330 | 98.205 | 107.725 | 95.422 | 107.725 |
| repo-clone | 5 | 172.902 | 166.953 | 201.817 | 160.943 | 201.817 |
| issue-create | 5 | 155.644 | 153.253 | 162.523 | 152.037 | 162.523 |
| issue-list | 5 | 69.347 | 67.596 | 74.844 | 65.420 | 74.844 |
| issue-view | 5 | 95.410 | 96.042 | 98.285 | 90.680 | 98.285 |
| pr-create | 5 | 261.660 | 255.046 | 290.527 | 248.418 | 290.527 |
| pr-list | 5 | 90.189 | 82.714 | 120.753 | 80.447 | 120.753 |
| pr-view | 5 | 147.419 | 148.050 | 151.626 | 143.974 | 151.626 |
| pr-merge | 5 | 148.629 | 149.101 | 150.290 | 145.620 | 150.290 |
| workflow-list | 5 | 63.252 | 62.600 | 65.562 | 61.770 | 65.562 |
| workflow-run | 5 | 103.472 | 103.038 | 105.076 | 102.623 | 105.076 |
| run-view | 5 | 141.508 | 143.368 | 145.585 | 136.118 | 145.585 |


<!-- trace-bench:7a175e60c03b79c2e463fbe4679fc07bc064fc97 -->
## 2026-04-22 02:37:40 UTC

- PR: [#1222](https://github.com/pingcap/agent-git-service/pull/1222) security: audit follow-ups from Issue #1217
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T02:35:36Z
- Merge commit: `7a175e60c03b79c2e463fbe4679fc07bc064fc97`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24757229476)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 56.305 | 55.827 | 62.256 | 51.219 | 62.256 |
| auth-status | 5 | 54.294 | 53.821 | 55.809 | 53.357 | 55.809 |
| auth-logout | 5 | 45.993 | 45.315 | 49.647 | 43.167 | 49.647 |
| repo-create | 5 | 69.406 | 68.844 | 76.178 | 64.955 | 76.178 |
| repo-view | 5 | 106.354 | 102.958 | 124.746 | 99.042 | 124.746 |
| repo-clone | 5 | 172.172 | 171.980 | 174.472 | 171.034 | 174.472 |
| issue-create | 5 | 163.838 | 163.343 | 171.723 | 159.402 | 171.723 |
| issue-list | 5 | 71.661 | 71.816 | 75.462 | 68.755 | 75.462 |
| issue-view | 5 | 94.557 | 94.604 | 97.575 | 91.842 | 97.575 |
| pr-create | 5 | 269.124 | 265.493 | 275.770 | 264.996 | 275.770 |
| pr-list | 5 | 88.709 | 86.897 | 101.688 | 81.972 | 101.688 |
| pr-view | 5 | 155.753 | 155.192 | 163.873 | 151.162 | 163.873 |
| pr-merge | 5 | 157.999 | 156.912 | 161.957 | 155.390 | 161.957 |
| workflow-list | 5 | 64.489 | 63.776 | 69.325 | 61.820 | 69.325 |
| workflow-run | 5 | 128.581 | 114.417 | 187.499 | 109.187 | 187.499 |
| run-view | 5 | 188.827 | 149.486 | 338.380 | 144.586 | 338.380 |


<!-- trace-bench:31403667f396218d1793c4a00386d0a063715d3d -->
## 2026-04-22 05:54:07 UTC

- PR: [#1227](https://github.com/pingcap/agent-git-service/pull/1227) perf: cut RPC count on hot list endpoints (N+1 + serial-git fixes)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T05:52:03Z
- Merge commit: `31403667f396218d1793c4a00386d0a063715d3d`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24762584032)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 53.407 | 51.316 | 61.918 | 48.972 | 61.918 |
| auth-status | 5 | 50.159 | 50.081 | 52.938 | 47.786 | 52.938 |
| auth-logout | 5 | 36.815 | 36.587 | 37.571 | 36.476 | 37.571 |
| repo-create | 5 | 60.715 | 60.893 | 62.003 | 59.496 | 62.003 |
| repo-view | 5 | 85.132 | 84.108 | 90.451 | 80.180 | 90.451 |
| repo-clone | 5 | 181.052 | 181.412 | 206.857 | 166.358 | 206.857 |
| issue-create | 5 | 152.623 | 151.528 | 155.620 | 149.840 | 155.620 |
| issue-list | 5 | 71.776 | 70.340 | 77.229 | 68.020 | 77.229 |
| issue-view | 5 | 92.072 | 91.576 | 97.257 | 88.863 | 97.257 |
| pr-create | 5 | 258.615 | 250.960 | 289.708 | 247.842 | 289.708 |
| pr-list | 5 | 87.244 | 80.054 | 124.025 | 74.744 | 124.025 |
| pr-view | 5 | 141.702 | 140.507 | 144.190 | 139.842 | 144.190 |
| pr-merge | 5 | 305.632 | 154.975 | 885.751 | 154.491 | 885.751 |
| workflow-list | 5 | 62.906 | 62.537 | 64.774 | 61.332 | 64.774 |
| workflow-run | 5 | 110.609 | 109.890 | 113.352 | 108.040 | 113.352 |
| run-view | 5 | 145.315 | 145.374 | 146.063 | 144.202 | 146.063 |


<!-- trace-bench:ed8b703ee409c569d492ef7f1a403faf7a4a8951 -->
## 2026-04-22 06:51:43 UTC

- PR: [#1229](https://github.com/pingcap/agent-git-service/pull/1229) fix(service): race-safe ensureAdminsTeamTx (closes #1228)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T06:49:37Z
- Merge commit: `ed8b703ee409c569d492ef7f1a403faf7a4a8951`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24764511731)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 51.547 | 51.589 | 52.851 | 49.508 | 52.851 |
| auth-status | 5 | 52.854 | 52.423 | 54.170 | 51.751 | 54.170 |
| auth-logout | 5 | 44.057 | 43.198 | 46.672 | 42.140 | 46.672 |
| repo-create | 5 | 66.399 | 67.399 | 67.871 | 63.016 | 67.871 |
| repo-view | 5 | 90.461 | 88.348 | 100.999 | 84.657 | 100.999 |
| repo-clone | 5 | 165.774 | 165.751 | 173.324 | 158.662 | 173.324 |
| issue-create | 5 | 151.859 | 151.759 | 161.596 | 146.421 | 161.596 |
| issue-list | 5 | 68.384 | 67.624 | 72.255 | 66.619 | 72.255 |
| issue-view | 5 | 89.681 | 88.959 | 92.223 | 87.031 | 92.223 |
| pr-create | 5 | 255.053 | 246.143 | 289.937 | 241.218 | 289.937 |
| pr-list | 5 | 82.198 | 81.875 | 86.259 | 78.594 | 86.259 |
| pr-view | 5 | 145.821 | 147.739 | 148.061 | 140.324 | 148.061 |
| pr-merge | 5 | 147.565 | 147.088 | 150.509 | 144.418 | 150.509 |
| workflow-list | 5 | 67.706 | 62.614 | 90.923 | 58.146 | 90.923 |
| workflow-run | 5 | 103.131 | 104.405 | 105.153 | 99.058 | 105.153 |
| run-view | 5 | 140.315 | 139.877 | 146.094 | 137.539 | 146.094 |


<!-- trace-bench:4faecd1b37b0536c92cd3d3d0e20d8509adfa59a -->
## 2026-04-22 07:13:21 UTC

- PR: [#1231](https://github.com/pingcap/agent-git-service/pull/1231) security: bound tidbcloud error body to 64KB (closes #1219)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T07:11:01Z
- Merge commit: `4faecd1b37b0536c92cd3d3d0e20d8509adfa59a`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24765293733)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 56.230 | 55.944 | 59.113 | 54.128 | 59.113 |
| auth-status | 5 | 58.627 | 58.354 | 59.903 | 57.584 | 59.903 |
| auth-logout | 5 | 48.746 | 46.589 | 58.159 | 45.134 | 58.159 |
| repo-create | 5 | 69.690 | 69.903 | 71.862 | 67.848 | 71.862 |
| repo-view | 5 | 104.030 | 102.163 | 111.818 | 99.976 | 111.818 |
| repo-clone | 5 | 182.292 | 183.860 | 185.441 | 177.066 | 185.441 |
| issue-create | 5 | 163.205 | 161.865 | 169.518 | 159.303 | 169.518 |
| issue-list | 5 | 75.563 | 74.413 | 84.141 | 70.082 | 84.141 |
| issue-view | 5 | 96.563 | 96.117 | 99.130 | 95.155 | 99.130 |
| pr-create | 5 | 283.291 | 271.084 | 328.076 | 268.354 | 328.076 |
| pr-list | 5 | 104.296 | 97.970 | 129.417 | 84.028 | 129.417 |
| pr-view | 5 | 157.644 | 157.034 | 160.810 | 154.726 | 160.810 |
| pr-merge | 5 | 159.502 | 159.846 | 161.998 | 155.997 | 161.998 |
| workflow-list | 5 | 64.817 | 65.574 | 67.674 | 60.166 | 67.674 |
| workflow-run | 5 | 124.172 | 118.592 | 149.659 | 115.647 | 149.659 |
| run-view | 5 | 156.218 | 156.580 | 159.319 | 153.384 | 159.319 |


<!-- trace-bench:cfed01112ac7aa35f6c0221d8b057e9ed1c098d5 -->
## 2026-04-22 07:15:25 UTC

- PR: [#1230](https://github.com/pingcap/agent-git-service/pull/1230) security: bound db9backend JSON decoder to 1MB (closes #1221)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T07:11:08Z
- Merge commit: `cfed01112ac7aa35f6c0221d8b057e9ed1c098d5`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24765298348)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 53.890 | 53.856 | 55.483 | 52.014 | 55.483 |
| auth-status | 5 | 57.751 | 58.590 | 59.382 | 53.615 | 59.382 |
| auth-logout | 5 | 42.520 | 42.250 | 44.120 | 41.324 | 44.120 |
| repo-create | 5 | 65.472 | 65.534 | 67.173 | 63.805 | 67.173 |
| repo-view | 5 | 91.493 | 92.002 | 92.727 | 89.496 | 92.727 |
| repo-clone | 5 | 171.186 | 172.618 | 174.281 | 165.912 | 174.281 |
| issue-create | 5 | 149.209 | 149.835 | 154.296 | 142.186 | 154.296 |
| issue-list | 5 | 68.675 | 68.564 | 69.137 | 68.143 | 69.137 |
| issue-view | 5 | 87.987 | 87.561 | 92.497 | 85.680 | 92.497 |
| pr-create | 5 | 257.423 | 252.409 | 296.058 | 241.808 | 296.058 |
| pr-list | 5 | 87.298 | 83.712 | 110.236 | 76.914 | 110.236 |
| pr-view | 5 | 144.977 | 147.452 | 149.258 | 140.287 | 149.258 |
| pr-merge | 5 | 154.340 | 154.132 | 158.733 | 147.279 | 158.733 |
| workflow-list | 5 | 61.501 | 60.920 | 63.965 | 60.642 | 63.965 |
| workflow-run | 5 | 113.369 | 108.112 | 138.273 | 100.951 | 138.273 |
| run-view | 5 | 137.238 | 136.464 | 140.256 | 134.317 | 140.256 |


<!-- trace-bench:8982a36d4237c2954f80cb3592042883f6b91ca5 -->
## 2026-04-22 09:48:58 UTC

- PR: [#1239](https://github.com/pingcap/agent-git-service/pull/1239) fix(git): GET/DELETE /git/refs/* and GET /git/matching-refs/* for custom namespaces
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T09:47:00Z
- Merge commit: `8982a36d4237c2954f80cb3592042883f6b91ca5`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24771698072)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 44.571 | 44.093 | 47.097 | 43.637 | 47.097 |
| auth-status | 5 | 46.472 | 46.265 | 47.279 | 45.829 | 47.279 |
| auth-logout | 5 | 37.935 | 37.275 | 41.602 | 35.904 | 41.602 |
| repo-create | 5 | 56.175 | 55.525 | 60.795 | 53.447 | 60.795 |
| repo-view | 5 | 79.954 | 80.330 | 81.917 | 77.150 | 81.917 |
| repo-clone | 5 | 149.663 | 144.214 | 176.785 | 140.720 | 176.785 |
| issue-create | 5 | 130.319 | 129.321 | 137.819 | 126.583 | 137.819 |
| issue-list | 5 | 60.375 | 60.728 | 63.273 | 57.453 | 63.273 |
| issue-view | 5 | 77.384 | 77.469 | 79.948 | 74.363 | 79.948 |
| pr-create | 5 | 219.325 | 208.280 | 260.424 | 206.002 | 260.424 |
| pr-list | 5 | 81.841 | 76.974 | 108.298 | 69.510 | 108.298 |
| pr-view | 5 | 123.970 | 123.884 | 128.995 | 120.183 | 128.995 |
| pr-merge | 5 | 128.992 | 124.844 | 149.908 | 121.855 | 149.908 |
| workflow-list | 5 | 55.129 | 55.362 | 56.935 | 53.854 | 56.935 |
| workflow-run | 5 | 98.306 | 95.690 | 124.986 | 83.477 | 124.986 |
| run-view | 5 | 123.610 | 123.463 | 126.927 | 121.618 | 126.927 |


<!-- trace-bench:c8208305b16c977011d8d3a72b67680c714f9623 -->
## 2026-04-22 09:51:00 UTC

- PR: [#1238](https://github.com/pingcap/agent-git-service/pull/1238) fix(git): reject non-fast-forward pushes to custom refs via pre-receive hook
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T09:47:27Z
- Merge commit: `c8208305b16c977011d8d3a72b67680c714f9623`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24771716484)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 45.346 | 44.720 | 47.251 | 44.226 | 47.251 |
| auth-status | 5 | 46.714 | 46.809 | 47.867 | 45.439 | 47.867 |
| auth-logout | 5 | 37.275 | 36.692 | 38.806 | 36.178 | 38.806 |
| repo-create | 5 | 56.705 | 56.863 | 58.160 | 54.865 | 58.160 |
| repo-view | 5 | 81.071 | 78.599 | 88.336 | 75.791 | 88.336 |
| repo-clone | 5 | 152.416 | 145.716 | 182.839 | 143.269 | 182.839 |
| issue-create | 5 | 132.587 | 131.163 | 135.993 | 129.192 | 135.993 |
| issue-list | 5 | 61.900 | 61.735 | 63.109 | 60.844 | 63.109 |
| issue-view | 5 | 79.106 | 78.399 | 82.428 | 77.845 | 82.428 |
| pr-create | 5 | 215.271 | 213.187 | 221.517 | 208.415 | 221.517 |
| pr-list | 5 | 71.002 | 66.875 | 88.111 | 65.524 | 88.111 |
| pr-view | 5 | 120.987 | 121.105 | 122.412 | 119.366 | 122.412 |
| pr-merge | 5 | 116.896 | 117.114 | 118.835 | 114.593 | 118.835 |
| workflow-list | 5 | 51.228 | 51.132 | 53.116 | 48.961 | 53.116 |
| workflow-run | 5 | 86.835 | 87.926 | 89.752 | 83.399 | 89.752 |
| run-view | 5 | 123.494 | 117.206 | 152.350 | 114.962 | 152.350 |


<!-- trace-bench:0b87fffc2142780a07b6efb9811f658f2c990985 -->
## 2026-04-22 10:04:26 UTC

- PR: [#1237](https://github.com/pingcap/agent-git-service/pull/1237) fix(git): atomic POST /git/refs — return 422 on duplicate ref
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T10:02:11Z
- Merge commit: `0b87fffc2142780a07b6efb9811f658f2c990985`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24772333833)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 55.474 | 53.669 | 62.087 | 53.639 | 62.087 |
| auth-status | 5 | 55.896 | 55.453 | 58.668 | 54.848 | 58.668 |
| auth-logout | 5 | 43.427 | 44.047 | 44.924 | 40.689 | 44.924 |
| repo-create | 5 | 69.639 | 69.086 | 72.475 | 67.918 | 72.475 |
| repo-view | 5 | 101.454 | 96.746 | 118.731 | 95.960 | 118.731 |
| repo-clone | 5 | 179.241 | 177.485 | 187.782 | 173.054 | 187.782 |
| issue-create | 5 | 156.689 | 157.680 | 161.287 | 151.696 | 161.287 |
| issue-list | 5 | 70.331 | 70.380 | 72.476 | 68.932 | 72.476 |
| issue-view | 5 | 93.624 | 94.182 | 96.587 | 91.133 | 96.587 |
| pr-create | 5 | 269.118 | 262.870 | 300.791 | 251.817 | 300.791 |
| pr-list | 5 | 82.669 | 82.616 | 84.699 | 81.589 | 84.699 |
| pr-view | 5 | 151.053 | 152.209 | 153.220 | 146.379 | 153.220 |
| pr-merge | 5 | 152.505 | 153.246 | 155.625 | 149.276 | 155.625 |
| workflow-list | 5 | 62.510 | 61.639 | 65.763 | 60.284 | 65.763 |
| workflow-run | 5 | 112.841 | 106.672 | 140.771 | 103.364 | 140.771 |
| run-view | 5 | 145.196 | 142.587 | 155.223 | 141.452 | 155.223 |


<!-- trace-bench:547a38f64ffe0797e345970e3aedcea19c4ad429 -->
## 2026-04-22 11:11:04 UTC

- PR: [#1236](https://github.com/pingcap/agent-git-service/pull/1236) refactor: consolidate HTTP error body reading patterns
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T10:08:41Z
- Merge commit: `547a38f64ffe0797e345970e3aedcea19c4ad429`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24772607725)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 46.259 | 46.135 | 49.187 | 44.374 | 49.187 |
| auth-status | 5 | 50.480 | 48.912 | 58.166 | 46.949 | 58.166 |
| auth-logout | 5 | 38.048 | 38.078 | 40.311 | 36.004 | 40.311 |
| repo-create | 5 | 56.988 | 56.508 | 60.378 | 53.679 | 60.378 |
| repo-view | 5 | 82.658 | 77.795 | 105.825 | 72.364 | 105.825 |
| repo-clone | 5 | 140.711 | 140.731 | 144.529 | 138.230 | 144.529 |
| issue-create | 5 | 128.789 | 126.466 | 135.257 | 123.782 | 135.257 |
| issue-list | 5 | 60.349 | 59.754 | 63.877 | 58.476 | 63.877 |
| issue-view | 5 | 77.833 | 77.820 | 78.905 | 76.648 | 78.905 |
| pr-create | 5 | 214.988 | 209.165 | 240.441 | 206.953 | 240.441 |
| pr-list | 5 | 69.448 | 68.633 | 70.916 | 68.282 | 70.916 |
| pr-view | 5 | 121.208 | 121.792 | 126.514 | 116.950 | 126.514 |
| pr-merge | 5 | 119.279 | 118.972 | 125.395 | 114.863 | 125.395 |
| workflow-list | 5 | 53.453 | 53.629 | 54.354 | 52.119 | 54.354 |
| workflow-run | 5 | 98.561 | 95.152 | 116.784 | 91.025 | 116.784 |
| run-view | 5 | 121.830 | 120.670 | 125.506 | 119.632 | 125.506 |


<!-- trace-bench:05b3d37bf7c6ed4d06907e103a5279f24c427c2a -->
## 2026-04-22 16:33:17 UTC

- PR: [#1241](https://github.com/pingcap/agent-git-service/pull/1241) fix: align large git push handling with GitHub
- PR resolution: resolved
- Author: @zhangyangyu
- PR merged at: 2026-04-22T16:31:02Z
- Merge commit: `05b3d37bf7c6ed4d06907e103a5279f24c427c2a`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24790151443)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 54.969 | 54.850 | 56.452 | 54.000 | 56.452 |
| auth-status | 5 | 56.035 | 55.625 | 57.995 | 54.459 | 57.995 |
| auth-logout | 5 | 44.490 | 44.149 | 45.825 | 43.062 | 45.825 |
| repo-create | 5 | 68.938 | 68.935 | 71.110 | 67.433 | 71.110 |
| repo-view | 5 | 99.143 | 96.791 | 113.045 | 92.630 | 113.045 |
| repo-clone | 5 | 174.047 | 174.722 | 178.624 | 170.238 | 178.624 |
| issue-create | 5 | 150.330 | 148.950 | 156.970 | 144.792 | 156.970 |
| issue-list | 5 | 69.705 | 69.639 | 72.030 | 66.857 | 72.030 |
| issue-view | 5 | 89.984 | 89.357 | 93.758 | 86.725 | 93.758 |
| pr-create | 5 | 266.873 | 261.592 | 290.721 | 253.207 | 290.721 |
| pr-list | 5 | 83.277 | 82.999 | 88.737 | 78.676 | 88.737 |
| pr-view | 5 | 148.655 | 148.794 | 157.782 | 141.357 | 157.782 |
| pr-merge | 5 | 154.974 | 155.585 | 156.480 | 153.237 | 156.480 |
| workflow-list | 5 | 64.877 | 64.397 | 66.580 | 63.735 | 66.580 |
| workflow-run | 5 | 119.070 | 112.629 | 143.838 | 107.918 | 143.838 |
| run-view | 5 | 142.771 | 142.331 | 145.922 | 140.851 | 145.922 |


<!-- trace-bench:487b8bdc01542ac2ce63947a10da8ecb09c495ab -->
## 2026-04-22 17:19:54 UTC

- PR: [#1243](https://github.com/pingcap/agent-git-service/pull/1243) fix(git-refs): strict-review follow-ups for #1237 / #1238 / #1239
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T17:17:49Z
- Merge commit: `487b8bdc01542ac2ce63947a10da8ecb09c495ab`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24792291764)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 57.588 | 57.394 | 60.669 | 55.283 | 60.669 |
| auth-status | 5 | 56.881 | 57.467 | 60.787 | 52.792 | 60.787 |
| auth-logout | 5 | 45.077 | 45.398 | 47.467 | 42.916 | 47.467 |
| repo-create | 5 | 71.459 | 72.613 | 75.970 | 66.787 | 75.970 |
| repo-view | 5 | 94.705 | 95.691 | 97.109 | 90.814 | 97.109 |
| repo-clone | 5 | 184.351 | 178.601 | 211.695 | 171.399 | 211.695 |
| issue-create | 5 | 155.561 | 153.998 | 161.310 | 152.460 | 161.310 |
| issue-list | 5 | 73.348 | 71.583 | 81.253 | 69.203 | 81.253 |
| issue-view | 5 | 95.410 | 94.472 | 98.629 | 92.876 | 98.629 |
| pr-create | 5 | 273.683 | 266.835 | 301.748 | 259.412 | 301.748 |
| pr-list | 5 | 91.976 | 84.795 | 115.953 | 83.516 | 115.953 |
| pr-view | 5 | 155.565 | 156.260 | 161.048 | 149.006 | 161.048 |
| pr-merge | 5 | 167.996 | 172.870 | 187.700 | 149.821 | 187.700 |
| workflow-list | 5 | 61.818 | 60.987 | 64.744 | 60.169 | 64.744 |
| workflow-run | 5 | 116.751 | 112.125 | 135.550 | 104.022 | 135.550 |
| run-view | 5 | 142.242 | 142.016 | 147.087 | 137.868 | 147.087 |


<!-- trace-bench:728dc534a02d91c8b3d419f4353e7f481a3d2d1e -->
## 2026-04-22 18:57:24 UTC

- PR: [#1261](https://github.com/pingcap/agent-git-service/pull/1261) fix(service): unify tenantKey — multi-tenant isolation was broken (closes #1244)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T18:55:12Z
- Merge commit: `728dc534a02d91c8b3d419f4353e7f481a3d2d1e`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24796760674)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 45.737 | 45.468 | 46.857 | 44.544 | 46.857 |
| auth-status | 5 | 47.880 | 48.737 | 49.502 | 45.870 | 49.502 |
| auth-logout | 5 | 35.903 | 35.826 | 37.179 | 34.976 | 37.179 |
| repo-create | 5 | 58.815 | 58.907 | 60.910 | 57.315 | 60.910 |
| repo-view | 5 | 79.333 | 79.094 | 81.897 | 76.407 | 81.897 |
| repo-clone | 5 | 156.985 | 149.345 | 182.273 | 145.788 | 182.273 |
| issue-create | 5 | 140.856 | 139.534 | 145.050 | 137.936 | 145.050 |
| issue-list | 5 | 61.657 | 61.632 | 64.152 | 58.881 | 64.152 |
| issue-view | 5 | 83.481 | 83.953 | 84.571 | 81.541 | 84.571 |
| pr-create | 5 | 244.584 | 236.822 | 263.260 | 228.997 | 263.260 |
| pr-list | 5 | 79.394 | 73.881 | 101.735 | 72.872 | 101.735 |
| pr-view | 5 | 135.182 | 132.959 | 144.800 | 131.718 | 144.800 |
| pr-merge | 5 | 140.721 | 140.610 | 142.590 | 138.725 | 142.590 |
| workflow-list | 5 | 54.695 | 54.043 | 56.859 | 52.847 | 56.859 |
| workflow-run | 5 | 94.350 | 94.065 | 97.286 | 92.534 | 97.286 |
| run-view | 5 | 132.228 | 129.267 | 151.460 | 123.467 | 151.460 |


<!-- trace-bench:ed1c3be827783ab270ed8d13ac81928c65939082 -->
## 2026-04-22 19:57:13 UTC

- PR: [#1269](https://github.com/pingcap/agent-git-service/pull/1269) perf(gitstore): add DiffNumStats helper; route PRDiffStats through it (closes #1250)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T19:54:45Z
- Merge commit: `ed1c3be827783ab270ed8d13ac81928c65939082`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24799469985)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 57.731 | 58.065 | 61.430 | 53.539 | 61.430 |
| auth-status | 5 | 57.870 | 57.619 | 60.035 | 56.869 | 60.035 |
| auth-logout | 5 | 43.710 | 44.507 | 45.491 | 41.082 | 45.491 |
| repo-create | 5 | 71.131 | 69.060 | 80.577 | 66.758 | 80.577 |
| repo-view | 5 | 98.878 | 96.220 | 117.892 | 84.182 | 117.892 |
| repo-clone | 5 | 162.158 | 163.068 | 172.386 | 154.653 | 172.386 |
| issue-create | 5 | 152.729 | 150.282 | 163.101 | 147.209 | 163.101 |
| issue-list | 5 | 71.602 | 67.037 | 83.547 | 66.433 | 83.547 |
| issue-view | 5 | 91.145 | 93.261 | 95.008 | 86.158 | 95.008 |
| pr-create | 5 | 259.046 | 259.198 | 279.586 | 246.482 | 279.586 |
| pr-list | 5 | 85.264 | 81.241 | 111.939 | 72.995 | 111.939 |
| pr-view | 5 | 139.720 | 140.830 | 142.389 | 136.450 | 142.389 |
| pr-merge | 5 | 153.373 | 150.354 | 163.031 | 147.096 | 163.031 |
| workflow-list | 5 | 58.922 | 58.888 | 63.376 | 55.757 | 63.376 |
| workflow-run | 5 | 104.191 | 103.047 | 111.808 | 98.453 | 111.808 |
| run-view | 5 | 147.625 | 140.335 | 178.425 | 137.187 | 178.425 |


<!-- trace-bench:17332b259db9b4d914852ce3ab32b7c501f35ebb -->
## 2026-04-22 19:59:28 UTC

- PR: [#1263](https://github.com/pingcap/agent-git-service/pull/1263) perf(rest): SearchRepos uses cached RepoDiskUsageKB (closes #1252)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T19:55:09Z
- Merge commit: `17332b259db9b4d914852ce3ab32b7c501f35ebb`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24799488216)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 54.353 | 54.005 | 55.418 | 53.779 | 55.418 |
| auth-status | 5 | 59.865 | 58.758 | 67.338 | 56.470 | 67.338 |
| auth-logout | 5 | 44.883 | 45.087 | 45.806 | 43.563 | 45.806 |
| repo-create | 5 | 70.113 | 70.909 | 73.144 | 66.615 | 73.144 |
| repo-view | 5 | 102.994 | 101.358 | 110.394 | 97.891 | 110.394 |
| repo-clone | 5 | 179.025 | 180.600 | 185.650 | 170.947 | 185.650 |
| issue-create | 5 | 170.444 | 168.660 | 185.201 | 161.636 | 185.201 |
| issue-list | 5 | 73.981 | 74.304 | 75.413 | 71.406 | 75.413 |
| issue-view | 5 | 99.210 | 99.617 | 108.916 | 90.171 | 108.916 |
| pr-create | 5 | 277.559 | 277.896 | 295.980 | 265.833 | 295.980 |
| pr-list | 5 | 91.764 | 92.187 | 94.122 | 89.354 | 94.122 |
| pr-view | 5 | 160.106 | 159.653 | 167.379 | 155.946 | 167.379 |
| pr-merge | 5 | 165.753 | 160.009 | 189.144 | 158.099 | 189.144 |
| workflow-list | 5 | 67.680 | 68.886 | 69.815 | 63.599 | 69.815 |
| workflow-run | 5 | 125.349 | 122.290 | 145.762 | 114.258 | 145.762 |
| run-view | 5 | 154.355 | 157.114 | 159.048 | 148.002 | 159.048 |


<!-- trace-bench:26450f8cca0485dc8287c0b5d01772325759798e -->
## 2026-04-22 20:09:57 UTC

- PR: [#1270](https://github.com/pingcap/agent-git-service/pull/1270) fix(gitstore): validate ref names and SHAs before shelling out (closes #1246)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T20:07:43Z
- Merge commit: `26450f8cca0485dc8287c0b5d01772325759798e`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24800053817)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 53.081 | 52.736 | 54.585 | 51.655 | 54.585 |
| auth-status | 5 | 55.112 | 54.860 | 57.931 | 53.057 | 57.931 |
| auth-logout | 5 | 43.149 | 42.719 | 45.094 | 42.270 | 45.094 |
| repo-create | 5 | 67.982 | 66.541 | 72.307 | 64.660 | 72.307 |
| repo-view | 5 | 92.071 | 91.225 | 93.490 | 91.051 | 93.490 |
| repo-clone | 5 | 163.290 | 157.408 | 196.493 | 151.815 | 196.493 |
| issue-create | 5 | 145.534 | 145.389 | 148.689 | 141.805 | 148.689 |
| issue-list | 5 | 69.787 | 64.983 | 89.707 | 62.131 | 89.707 |
| issue-view | 5 | 84.339 | 83.740 | 87.551 | 81.804 | 87.551 |
| pr-create | 5 | 249.084 | 248.198 | 267.419 | 238.190 | 267.419 |
| pr-list | 5 | 80.701 | 74.579 | 107.925 | 72.637 | 107.925 |
| pr-view | 5 | 134.829 | 135.063 | 136.944 | 132.870 | 136.944 |
| pr-merge | 5 | 143.710 | 142.981 | 146.960 | 142.451 | 146.960 |
| workflow-list | 5 | 55.952 | 55.505 | 58.134 | 54.218 | 58.134 |
| workflow-run | 5 | 100.256 | 96.600 | 106.912 | 95.781 | 106.912 |
| run-view | 5 | 137.612 | 137.319 | 141.154 | 135.074 | 141.154 |


<!-- trace-bench:5b7a9c32fe01d2a7974e9b923d634aa743f24058 -->
## 2026-04-22 20:12:17 UTC

- PR: [#1262](https://github.com/pingcap/agent-git-service/pull/1262) perf(gitstore): ListDir uses ls-tree -l (closes #1251)
- PR resolution: resolved
- Author: @ngaut
- PR merged at: 2026-04-22T20:07:55Z
- Merge commit: `5b7a9c32fe01d2a7974e9b923d634aa743f24058`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24800062611)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 56.126 | 56.883 | 59.487 | 52.860 | 59.487 |
| auth-status | 5 | 59.552 | 60.099 | 61.429 | 56.529 | 61.429 |
| auth-logout | 5 | 46.942 | 46.977 | 49.538 | 45.089 | 49.538 |
| repo-create | 5 | 72.341 | 72.559 | 76.058 | 68.702 | 76.058 |
| repo-view | 5 | 111.658 | 109.822 | 142.389 | 89.695 | 142.389 |
| repo-clone | 5 | 167.775 | 167.561 | 173.921 | 163.698 | 173.921 |
| issue-create | 5 | 161.166 | 160.086 | 173.702 | 152.926 | 173.702 |
| issue-list | 5 | 66.872 | 66.642 | 69.210 | 64.957 | 69.210 |
| issue-view | 5 | 93.671 | 94.258 | 99.054 | 89.550 | 99.054 |
| pr-create | 5 | 277.494 | 272.507 | 292.401 | 268.460 | 292.401 |
| pr-list | 5 | 88.321 | 82.929 | 112.934 | 78.804 | 112.934 |
| pr-view | 5 | 155.122 | 152.912 | 168.302 | 148.021 | 168.302 |
| pr-merge | 5 | 157.055 | 155.833 | 161.906 | 152.221 | 161.906 |
| workflow-list | 5 | 60.699 | 60.328 | 62.177 | 59.451 | 62.177 |
| workflow-run | 5 | 124.379 | 120.356 | 150.652 | 111.541 | 150.652 |
| run-view | 5 | 154.268 | 153.209 | 157.877 | 151.141 | 157.877 |


<!-- trace-bench:783078f5be3070cb3a36c383528328ba12894322 -->
## 2026-04-22 20:25:43 UTC

- PR: [#1271](https://github.com/pingcap/agent-git-service/pull/1271) refactor: use plumbing.NewBranchReferenceName/NewTagReferenceName and shared constants (closes #1260)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T20:23:40Z
- Merge commit: `783078f5be3070cb3a36c383528328ba12894322`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24800768256)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 52.710 | 51.039 | 57.980 | 50.887 | 57.980 |
| auth-status | 5 | 54.789 | 52.291 | 62.993 | 51.592 | 62.993 |
| auth-logout | 5 | 42.765 | 43.036 | 43.233 | 42.064 | 43.233 |
| repo-create | 5 | 65.079 | 64.844 | 67.280 | 63.678 | 67.280 |
| repo-view | 5 | 92.697 | 91.560 | 98.230 | 90.443 | 98.230 |
| repo-clone | 5 | 162.170 | 154.082 | 193.474 | 152.825 | 193.474 |
| issue-create | 5 | 143.225 | 142.608 | 146.531 | 139.438 | 146.531 |
| issue-list | 5 | 63.007 | 62.287 | 66.785 | 61.012 | 66.785 |
| issue-view | 5 | 83.660 | 83.241 | 86.590 | 81.160 | 86.590 |
| pr-create | 5 | 242.876 | 235.410 | 274.448 | 229.552 | 274.448 |
| pr-list | 5 | 80.170 | 74.200 | 107.076 | 70.587 | 107.076 |
| pr-view | 5 | 139.271 | 135.206 | 155.415 | 131.493 | 155.415 |
| pr-merge | 5 | 151.307 | 143.973 | 177.800 | 140.342 | 177.800 |
| workflow-list | 5 | 54.909 | 54.025 | 59.669 | 52.760 | 59.669 |
| workflow-run | 5 | 97.304 | 95.793 | 107.215 | 92.514 | 107.215 |
| run-view | 5 | 135.161 | 135.790 | 139.774 | 126.969 | 139.774 |


<!-- trace-bench:660cd78dd3864266049669978b860b7aea3936b5 -->
## 2026-04-22 21:09:18 UTC

- PR: [#1272](https://github.com/pingcap/agent-git-service/pull/1272) fix(rest): decodeBodyStrict for write handlers; use errors.Is for EOF check (closes #1259)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T21:07:05Z
- Merge commit: `660cd78dd3864266049669978b860b7aea3936b5`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24802714030)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 58.175 | 57.065 | 60.582 | 56.155 | 60.582 |
| auth-status | 5 | 55.590 | 55.104 | 58.414 | 53.861 | 58.414 |
| auth-logout | 5 | 45.810 | 43.422 | 56.676 | 41.760 | 56.676 |
| repo-create | 5 | 66.936 | 65.932 | 71.590 | 62.953 | 71.590 |
| repo-view | 5 | 101.782 | 103.102 | 118.030 | 82.130 | 118.030 |
| repo-clone | 5 | 161.134 | 161.137 | 165.000 | 155.388 | 165.000 |
| issue-create | 5 | 142.353 | 142.432 | 146.229 | 138.573 | 146.229 |
| issue-list | 5 | 62.969 | 63.210 | 63.659 | 61.900 | 63.659 |
| issue-view | 5 | 85.129 | 84.631 | 89.328 | 80.397 | 89.328 |
| pr-create | 5 | 237.117 | 235.858 | 245.007 | 232.199 | 245.007 |
| pr-list | 5 | 74.398 | 74.034 | 79.661 | 70.087 | 79.661 |
| pr-view | 5 | 135.338 | 133.283 | 144.000 | 130.554 | 144.000 |
| pr-merge | 5 | 150.235 | 148.259 | 161.365 | 145.103 | 161.365 |
| workflow-list | 5 | 54.910 | 54.590 | 57.422 | 52.811 | 57.422 |
| workflow-run | 5 | 108.972 | 108.517 | 120.478 | 99.331 | 120.478 |
| run-view | 5 | 135.262 | 135.097 | 139.730 | 128.668 | 139.730 |


<!-- trace-bench:2dab8f6a27ee64c4d514280e285d5543bc384b48 -->
## 2026-04-22 22:59:54 UTC

- PR: [#1276](https://github.com/pingcap/agent-git-service/pull/1276) docs: update SSOT module contracts (#1248)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T22:57:50Z
- Merge commit: `2dab8f6a27ee64c4d514280e285d5543bc384b48`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24806979802)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 54.337 | 53.790 | 58.674 | 51.427 | 58.674 |
| auth-status | 5 | 56.657 | 53.502 | 64.849 | 51.579 | 64.849 |
| auth-logout | 5 | 42.896 | 42.108 | 45.704 | 41.896 | 45.704 |
| repo-create | 5 | 66.611 | 64.696 | 71.719 | 63.041 | 71.719 |
| repo-view | 5 | 95.724 | 96.056 | 99.435 | 90.602 | 99.435 |
| repo-clone | 5 | 178.711 | 172.586 | 205.646 | 167.417 | 205.646 |
| issue-create | 5 | 156.552 | 154.630 | 166.033 | 151.369 | 166.033 |
| issue-list | 5 | 68.993 | 68.264 | 71.819 | 67.355 | 71.819 |
| issue-view | 5 | 93.602 | 93.481 | 98.552 | 89.273 | 98.552 |
| pr-create | 5 | 254.037 | 254.342 | 260.334 | 247.905 | 260.334 |
| pr-list | 5 | 76.039 | 76.292 | 77.246 | 74.080 | 77.246 |
| pr-view | 5 | 146.044 | 146.242 | 147.581 | 143.929 | 147.581 |
| pr-merge | 5 | 150.750 | 150.836 | 154.081 | 146.778 | 154.081 |
| workflow-list | 5 | 62.255 | 60.878 | 65.419 | 60.322 | 65.419 |
| workflow-run | 5 | 101.199 | 101.607 | 104.501 | 96.210 | 104.501 |
| run-view | 5 | 143.724 | 137.865 | 165.232 | 135.965 | 165.232 |


<!-- trace-bench:e325c527dc81242895a27ee002c842f83fe22593 -->
## 2026-04-22 23:03:59 UTC

- PR: [#1275](https://github.com/pingcap/agent-git-service/pull/1275) fix: unify tenant context key - multi-tenant isolation (#1245)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-22T23:01:48Z
- Merge commit: `e325c527dc81242895a27ee002c842f83fe22593`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24807113103)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 52.709 | 53.666 | 54.364 | 50.128 | 54.364 |
| auth-status | 5 | 57.854 | 56.810 | 62.372 | 55.094 | 62.372 |
| auth-logout | 5 | 42.767 | 42.600 | 44.469 | 41.222 | 44.469 |
| repo-create | 5 | 72.374 | 72.424 | 77.735 | 68.383 | 77.735 |
| repo-view | 5 | 90.845 | 91.335 | 94.832 | 86.485 | 94.832 |
| repo-clone | 5 | 173.031 | 172.437 | 178.686 | 169.114 | 178.686 |
| issue-create | 5 | 170.610 | 168.953 | 185.670 | 161.302 | 185.670 |
| issue-list | 5 | 67.208 | 66.956 | 72.238 | 62.616 | 72.238 |
| issue-view | 5 | 86.898 | 87.218 | 89.349 | 83.997 | 89.349 |
| pr-create | 5 | 294.116 | 300.799 | 306.987 | 273.810 | 306.987 |
| pr-list | 5 | 88.854 | 86.098 | 94.912 | 84.964 | 94.912 |
| pr-view | 5 | 169.060 | 170.045 | 181.965 | 157.016 | 181.965 |
| pr-merge | 5 | 177.374 | 168.523 | 203.505 | 164.024 | 203.505 |
| workflow-list | 5 | 59.623 | 59.619 | 61.697 | 57.494 | 61.697 |
| workflow-run | 5 | 120.768 | 109.014 | 171.671 | 105.491 | 171.671 |
| run-view | 5 | 151.442 | 151.565 | 160.173 | 143.272 | 160.173 |


<!-- trace-bench:304deec99ab4ef42f16bbac379f83f2a42ee1151 -->
## 2026-04-23 00:56:53 UTC

- PR: [#1274](https://github.com/pingcap/agent-git-service/pull/1274) fix: resolve layer violations (#1256)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-23T00:54:39Z
- Merge commit: `304deec99ab4ef42f16bbac379f83f2a42ee1151`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24810622150)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 56.587 | 57.121 | 58.383 | 54.193 | 58.383 |
| auth-status | 5 | 56.016 | 55.843 | 58.191 | 54.035 | 58.191 |
| auth-logout | 5 | 45.132 | 45.034 | 47.560 | 43.642 | 47.560 |
| repo-create | 5 | 69.786 | 68.966 | 73.062 | 67.754 | 73.062 |
| repo-view | 5 | 106.418 | 99.976 | 134.234 | 92.241 | 134.234 |
| repo-clone | 5 | 176.031 | 176.823 | 177.944 | 173.160 | 177.944 |
| issue-create | 5 | 160.842 | 161.988 | 165.679 | 151.527 | 165.679 |
| issue-list | 5 | 69.946 | 71.729 | 72.350 | 66.670 | 72.350 |
| issue-view | 5 | 94.369 | 93.066 | 99.586 | 91.990 | 99.586 |
| pr-create | 5 | 253.026 | 253.298 | 258.343 | 246.416 | 258.343 |
| pr-list | 5 | 82.434 | 81.524 | 85.593 | 79.892 | 85.593 |
| pr-view | 5 | 144.066 | 145.762 | 148.754 | 136.846 | 148.754 |
| pr-merge | 5 | 156.704 | 158.310 | 159.367 | 151.868 | 159.367 |
| workflow-list | 5 | 60.325 | 58.040 | 65.950 | 55.593 | 65.950 |
| workflow-run | 5 | 114.574 | 108.808 | 141.182 | 103.437 | 141.182 |
| run-view | 5 | 144.256 | 143.969 | 147.769 | 139.353 | 147.769 |


<!-- trace-bench:f2c96c3bf1e07783af6cb19e9c131a0e6ad4a077 -->
## 2026-04-23 06:10:08 UTC

- PR: [#1273](https://github.com/pingcap/agent-git-service/pull/1273) fix: implement OAuth device code flow security (#1249)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-23T06:08:05Z
- Merge commit: `f2c96c3bf1e07783af6cb19e9c131a0e6ad4a077`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24819785101)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 54.875 | 55.524 | 56.625 | 51.958 | 56.625 |
| auth-status | 5 | 55.157 | 54.524 | 58.434 | 53.346 | 58.434 |
| auth-logout | 5 | 43.435 | 43.331 | 45.394 | 42.051 | 45.394 |
| repo-create | 5 | 66.351 | 65.822 | 71.319 | 63.193 | 71.319 |
| repo-view | 5 | 96.294 | 97.849 | 100.112 | 91.101 | 100.112 |
| repo-clone | 5 | 164.028 | 159.965 | 188.753 | 152.646 | 188.753 |
| issue-create | 5 | 150.206 | 149.442 | 156.714 | 146.396 | 156.714 |
| issue-list | 5 | 64.134 | 64.300 | 66.787 | 62.134 | 66.787 |
| issue-view | 5 | 90.261 | 90.510 | 95.927 | 83.170 | 95.927 |
| pr-create | 5 | 252.301 | 247.736 | 279.310 | 238.019 | 279.310 |
| pr-list | 5 | 76.658 | 76.703 | 79.384 | 75.053 | 79.384 |
| pr-view | 5 | 137.155 | 137.524 | 139.188 | 134.638 | 139.188 |
| pr-merge | 5 | 151.573 | 151.088 | 156.399 | 147.386 | 156.399 |
| workflow-list | 5 | 58.470 | 58.765 | 64.745 | 54.568 | 64.745 |
| workflow-run | 5 | 105.648 | 100.272 | 124.455 | 98.041 | 124.455 |
| run-view | 5 | 139.981 | 138.198 | 154.376 | 133.003 | 154.376 |


<!-- trace-bench:c046bd95b233eaf0ccd5a70cc118cc2cf10453a9 -->
## 2026-04-23 17:26:06 UTC

- PR: [#1290](https://github.com/pingcap/agent-git-service/pull/1290) fix: enable workflow execution in trace bench workflow
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-23T17:23:46Z
- Merge commit: `c046bd95b233eaf0ccd5a70cc118cc2cf10453a9`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24849044120)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 62.513 | 61.950 | 69.286 | 58.312 | 69.286 |
| auth-status | 5 | 61.697 | 62.189 | 63.632 | 58.971 | 63.632 |
| auth-logout | 5 | 47.510 | 47.010 | 53.189 | 44.227 | 53.189 |
| repo-create | 5 | 75.924 | 76.257 | 81.443 | 71.188 | 81.443 |
| repo-view | 5 | 97.287 | 90.279 | 127.879 | 87.195 | 127.879 |
| repo-clone | 5 | 166.470 | 166.276 | 167.991 | 165.587 | 167.991 |
| issue-create | 5 | 159.288 | 157.059 | 172.745 | 153.637 | 172.745 |
| issue-list | 5 | 68.485 | 67.882 | 71.105 | 66.675 | 71.105 |
| issue-view | 5 | 93.955 | 94.226 | 97.863 | 91.035 | 97.863 |
| pr-create | 5 | 279.058 | 282.378 | 311.178 | 257.203 | 311.178 |
| pr-list | 5 | 83.008 | 82.012 | 87.876 | 80.187 | 87.876 |
| pr-view | 5 | 152.954 | 153.088 | 157.268 | 149.493 | 157.268 |
| pr-merge | 5 | 156.989 | 156.604 | 164.456 | 151.980 | 164.456 |
| workflow-list | 5 | 68.187 | 65.046 | 78.373 | 61.933 | 78.373 |
| workflow-run | 5 | 210.545 | 201.693 | 280.858 | 153.885 | 280.858 |
| run-view | 5 | 169.065 | 157.737 | 192.574 | 153.154 | 192.574 |


<!-- trace-bench:c316d139ae088df31f1e00985ef789809c8079d1 -->
## 2026-04-23 17:47:58 UTC

- PR: [#1283](https://github.com/pingcap/agent-git-service/pull/1283) test: add regression test for issue #1281 (URL-encoded label deletion)
- PR resolution: resolved
- Author: @EricZequan
- PR merged at: 2026-04-23T17:45:49Z
- Merge commit: `c316d139ae088df31f1e00985ef789809c8079d1`
- Workflow run: [run](https://github.com/pingcap/agent-git-service/actions/runs/24850034364)
- Bench command: `scripts/bench-gh.sh --runs 5 --warmups 1`

| scenario | n | mean_ms | p50_ms | p95_ms | min_ms | max_ms |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| auth-login | 5 | 46.538 | 47.105 | 47.988 | 44.407 | 47.988 |
| auth-status | 5 | 47.242 | 46.519 | 50.513 | 44.834 | 50.513 |
| auth-logout | 5 | 37.533 | 36.650 | 40.467 | 35.984 | 40.467 |
| repo-create | 5 | 61.592 | 61.135 | 66.278 | 57.209 | 66.278 |
| repo-view | 5 | 80.028 | 79.269 | 82.430 | 78.311 | 82.430 |
| repo-clone | 5 | 150.972 | 150.963 | 155.321 | 148.400 | 155.321 |
| issue-create | 5 | 140.679 | 140.299 | 143.554 | 138.888 | 143.554 |
| issue-list | 5 | 61.802 | 61.733 | 63.365 | 60.592 | 63.365 |
| issue-view | 5 | 82.943 | 82.521 | 86.976 | 80.728 | 86.976 |
| pr-create | 5 | 243.327 | 237.672 | 273.019 | 230.588 | 273.019 |
| pr-list | 5 | 73.145 | 72.995 | 76.548 | 70.744 | 76.548 |
| pr-view | 5 | 140.936 | 140.669 | 161.861 | 128.504 | 161.861 |
| pr-merge | 5 | 141.621 | 141.701 | 143.552 | 140.164 | 143.552 |
| workflow-list | 5 | 54.759 | 54.567 | 60.404 | 51.189 | 60.404 |
| workflow-run | 5 | 198.846 | 173.579 | 282.250 | 140.788 | 282.250 |
| run-view | 5 | 135.520 | 134.382 | 149.942 | 127.625 | 149.942 |

