### README

Failing commands:

```bash
➜  test git:(master) ✗ dagger edit
2:01AM FTL system | invalid input: import failed: build constraints exclude all CUE files in github.com/toto-tata:
    cue.mod/usr/github.com/toto-tata/main.cue: package is toto, want toto-tata    environment=foo-bar
➜  test git:(master) ✗ dagger input list
2:01AM FTL system | failed to query environment: import failed: build constraints exclude all CUE files in github.com/toto-tata:
    cue.mod/usr/github.com/toto-tata/main.cue: package is toto, want toto-tata    environment=foo-bar
➜  test git:(master) ✗ dagger list
foo-bar /tmp/test/.dagger/env/foo-bar
➜  test git:(master) ✗ dagger edit -e foo-bar
2:02AM FTL system | invalid input: import failed: build constraints exclude all CUE files in github.com/toto-tata:
    cue.mod/usr/github.com/toto-tata/main.cue: package is toto, want toto-tata    environment=foo-bar
```