# Go Benchmarks

Continous Integration setups are great for verifying the integrity of a
codebase with binary tests (i.e. pass/fail), clearly indicating at what
revision a regression occurs. However, not all tests are strictly binary.
For example, you may want to track the binary size of your application.
You could write a test that fails when your binary size exceeds a certain
threshold. However, if your application is expected to gain in size by a
certain percentage for each commit then your test will periodically fail, and
you will have to continually reset the test threshold to get your CI to pass
again.
