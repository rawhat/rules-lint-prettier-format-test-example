```sh
quantas ~/code/prettier-bazel-format-test (main) δ bazel test :app.check
INFO: Analyzed target //:app.check_JavaScript_with_prettier (111 packages loaded, 5531 targets configured).
INFO: Found 1 test target...
Target //:app.check_JavaScript_with_prettier up-to-date:
  bazel-bin/app.check_JavaScript_with_prettier
INFO: Elapsed time: 0.392s, Critical Path: 0.08s
INFO: 10 processes: 6 internal, 3 linux-sandbox, 1 local.
INFO: Build completed successfully, 10 total actions
//:app.check_JavaScript_with_prettier                                    PASSED in 0.0s

Executed 1 out of 1 test: 1 test passes.
There were tests whose specified size is too big. Use the --test_verbose_timeout_warnings command line option to see which ones these are.
quantas ~/code/prettier-bazel-format-test (main) δ bazel run :app.check
INFO: Analyzed target //:app.check_JavaScript_with_prettier (0 packages loaded, 0 targets configured).
INFO: Found 1 target...
Target //:app.check_JavaScript_with_prettier up-to-date:
  bazel-bin/app.check_JavaScript_with_prettier
INFO: Elapsed time: 0.043s, Critical Path: 0.00s
INFO: 1 process: 1 internal.
INFO: Build completed successfully, 1 total action
INFO: Running command line: external/bazel_tools/tools/test/test-setup.sh ./app.check_JavaScript_with_prettier ./index.js
exec ${PAGER:-/usr/bin/less} "$0" || exit 1
Executing tests from //:app.check_JavaScript_with_prettier
-----------------------------------------------------------------------------
Checking formatting...
[warn] index.js
[warn] Code style issues found in the above file. Run Prettier with --write to fix.
Formatted JavaScript in 0m0.076s
FAILED: A formatter tool exited with code 123
Try running 'bazel run //:app.check_JavaScript_with_prettier ./index.js' to fix this.
```
