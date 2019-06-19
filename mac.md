# Getting started instructions for Mac

**Before you start**

Verify that Anaconda is installed in your HOME folder.
The path should be `/Users/<username>/anaconda3`.

> Replace `<username>` with your username.

Make sure that you have `git` or the `XCode command line tools` installed.

**Steps**

1. Open the Terminal.
2. Navigate to the workshop folder. For example, if the workshop folder is at `/Users/<username>/Workshops/WS_Anagni2019`

   ```bash
   cd ~/Workshops/WS_Anagni2019
   ```

3. Create an environment called "masonry".

   ```bash
   conda create -n masonry python=3.6 python.app
   ```
   > Don't forget `python.app`.

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

7. Navigate to `compas_tna-UI`. For example, if the folder is at `/Users/<username>/Workshops/compas_tna-UI`

   ```bash
   cd ~/Workshops/compas_tna-UI
   ```

8. Install the UI.

   > Shutdown Rhino first, if it is running.
   > Packages will be available next time you start Rhino.

   ```bash
   python -m compas_rhino.install_plugin TNA{d8bb2ef6-4539-4ba7-aa48-8ecadb23c229}
   ```

**Get help**

The fastest and most efficient way to get help with any of the above steps is to post your problem on the issue tracker.

https://github.com/BlockResearchGroup/WS_Anagni2019/issues


**Updates**

If you need to update one of the "masonry" packages (for example, because the guys providing support from Zurich made a change to the code of let's say `compas_assembly` :), do the following with the correct environment active (in this case, `masonry`).

```bash
pip install --upgrade git+https://github.com/BlockResearchGroup/compas_assembly.git#egg=compas_assembly
```

For the other packages, the procedure is the same, but no changes were made there!

```bash
pip install --upgrade git+https://github.com/BlockResearchGroup/compas_tna.git#egg=compas_tna
```

```bash
pip install --upgrade git+https://github.com/BlockResearchGroup/compas_rbe.git#egg=compas_rbe
```

There is no need to reinstall for Rhino, but the changes will only have effect next time you start Rhino.
