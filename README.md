# integrate-Tower-with-IntelliJIDEA
Integration of IntelliJ IDEA merge and diff tool with Tower app.


### Steps: ###
#### macOS ####
Integrations scripts are based on official documentation:
https://www.git-tower.com/help/guides/integration/custom-diff-tools/mac

1. Place files `CompareTools.plist` and `intellijidea.sh` into the `~/Library/Application Support/com.fournova.Tower3/CompareTools/` directory.
If you don't have `CompareTools` directory, just create it. (complete path to `CompareTools.plist` should be `~/Library/Application Support/com.fournova.Tower3/CompareTools/CompareTools.plist`)
2. Make `intellijidea.sh` executable by running command `chmod 755 ~/Library/Application\ Support/com.fournova.Tower3/CompareTools/intellijidea.sh` in your terminal.
3. Open `Tower.app`: Preferences -> Git Config, and select `IntelliJ IDEA` as merge and diff tool. Also you can select "Perform directory diff"

#### Windows ####
Integrations scripts are based on official documentation:
https://www.git-tower.com/help/guides/integration/custom-diff-tools/windows

1. Place file `CompareTool.json` into the `C:\Users\<Your User>\AppData\Local\fournova\Tower\Settings\CompareTools` directory.
   If you don't have `CompareTools` directory, just create it. (complete path to `CompareTool.json` should be `C:\Users\<Your User>\AppData\Local\fournova\Tower\Settings\CompareTools\CompareTool.json`)
2. Open `cmd.exe` with admin roots and execute command `setx /M PATH "C:\Program Files\JetBrains\IntelliJ IDEA\bin"` (WARNING!!! Your path to IntelliJ IDEA can be different).
3. Open `Tower.app`: Preferences -> Git Config, and select `IntelliJ IDEA` as merge and diff tool. Also you can select "Perform directory diff"
