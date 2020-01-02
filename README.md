# dune-promotion-stop-example

All promotions used to be run:
```
$ dune --version
1.11.4
$ dune runtest
Done: 0/0 (jobs: 0)File "a.expected", line 1, characters 0-0:
         git (internal) (exit 1)
(cd _build/default && /usr/bin/git diff --no-index --color=always -u a.expected a)
diff --git a/a.expected b/a
index 7898192..975fbec 100644
--- a/a.expected
+++ b/a
@@ -1 +1 @@
-a
+y
Done: 4/7 (jobs: 1)File "b.expected", line 1, characters 0-0:
         git (internal) (exit 1)
(cd _build/default && /usr/bin/git diff --no-index --color=always -u b.expected b)
diff --git a/b.expected b/b
index 6178079..b680253 100644
--- a/b.expected
+++ b/b
@@ -1 +1 @@
-b
+z
```

But in 2.0.0:
```
$ dune --version
n/a
$ dune runtest
Done: 0/0 (jobs: 0)File "a.expected", line 1, characters 0-0:
         git (internal) (exit 1)
(cd _build/default && /usr/bin/git diff --no-index --color=always -u a.expected a)
diff --git a/a.expected b/a
index 7898192..975fbec 100644
--- a/a.expected
+++ b/a
@@ -1 +1 @@
-a
+y
```
