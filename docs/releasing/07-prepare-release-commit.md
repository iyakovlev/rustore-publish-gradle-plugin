## Prepare Release Commit

1. Edit ./plugin/gradle.properties, remove '-alpha*' from the `VERSION_NAME` property
2. Make a *signed* commit:
   ```bash
   git commit -m "Release X.Y.Z"
   ```
3. Make a *signed* tag (check existing tags for message format):
   ```bash
   git tag -a "X.Y.Z" -m "X.Y.Z" 
   ```
4. Push all of our work to Github to make it official:
   ```bash
   git push --tags origin master
