# integrate-Tower-with-IntelliJIDEA
Integration of IntelliJ IDEA merge and diff tool with Tower app.

Integrations scripts are based on official documentation:
https://www.git-tower.com/help/guides/integration/custom-diff-tools/mac

### Steps: ###
#### macOS ####
1. Place files `CompareTools.plist` and `intellijidea.sh` into the `~/Library/Application Support/com.fournova.Tower3/CompareTools/` directory.
If you don't have `CompareTools` directory, just create it. (complete path to `CompareTools.plist` should be `~/Library/Application Support/com.fournova.Tower3/CompareTools/CompareTools.plist`)
2. Make `intellijidea.sh` executable by running command `chmod 755 ~/Library/Application\ Support/com.fournova.Tower3/CompareTools/intellijidea.sh` in your terminal.
3. Open `Tower.app`: Preferences -> Git Config, and select `IntelliJ IDEA` as merge and diff tool. Also you can select "Perform directory diff"

#### Windows ####
