# Getting started instructions for Windows

**Before you start**

Verify that Anaconda is installed in your HOME folder.
The path should be `C:\Users\<username>\Anaconda3`.

> Replace `<username>` with your username.

Make sure that you have `git` installed.

**Steps**

1. Run the Anaconda Prompt as administrator.
2. Navigate to the workshop folder. For example, if the workshop folder is at `C:\Users\<username>\Workshops\WS_Anagni2019`

   ```bash
   cd %USERPROFILE%\Workshops\WS_Anagni2019
   ```

3. Create an environment called "masonry".

   ```bash
   conda create -n masonry python=3.6
   ```

4. Activate the environment.

   ```bash
   conda activate masonry
   ```

5. Update the environment.

   ```bash
   conda env update -f environment.yml
   ```

6. Install for Rhino.

   > Shutdown Rhino first, if it is running.
   > Packages will be available next time you start Rhino.

   ```bash
   python -m compas_rhino.uninstall
   python -m compas_rhino.install -p compas compas_rhino compas_tna compas_assembly compas_rbe
   ```
   > For Rhino 5, add the flag `-v 5.0`.

7. Navigate to `compas_tna-UI`. For example, if the folder is at `C:\Users\<username>\Workshops\compas_tna-UI`

   ```bash
   cd %USERPROFILE%\Workshops\compas_tna-UI
   ```

8. Install the UI.

   > Shutdown Rhino first, if it is running.
   > Packages will be available next time you start Rhino.

   ```bash
   python -m compas_rhino.install_plugin TNA{d8bb2ef6-4539-4ba7-aa48-8ecadb23c229}
   ```
   > Sometimes the plugin commands only become available after you open the PythonScriptEditor. No need to keep it open afterwards.

**Get help**

The fastest and most efficient way to get help with any of the above steps is to post your problem on the issue tracker.

https://github.com/BlockResearchGroup/WS_Anagni2019/issues