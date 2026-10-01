# Palisade longitudinal fork

Base: commaai/openpilot `release-tici` (v0.10.0, comma 3).

Hyundai Palisade 2020-22 (HYUNDAI_PALISADE) already has `alphaLongitudinalAvailable = True`
upstream. The only thing hiding the toggle on a stock build is `IsReleaseBranch`, which is
true when the git branch name is in RELEASE_BRANCHES (system/version.py). This fork lives on
the branch `palisade-long`, so the toggle is visible:

Settings -> Developer -> "openpilot Longitudinal Control (Alpha)" -> enable, then reboot.

No source changes; the shipped prebuilt binaries are unchanged.
