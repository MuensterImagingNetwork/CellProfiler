## General
Bad key text.latex.preview in file C:\ProgramData\Anaconda3\envs\cellprofiler\lib\site-packages\matplotlib\mpl-data\stylelib\_classic_test.mplstyle, line 123 ('text.latex.preview : False')
You probably need to get an updated matplotlibrc file from
https://github.com/matplotlib/matplotlib/blob/v3.5.0/matplotlibrc.template
or from the matplotlib source distribution

Bad key mathtext.fallback_to_cm in file C:\ProgramData\Anaconda3\envs\cellprofiler\lib\site-packages\matplotlib\mpl-data\stylelib\_classic_test.mplstyle, line 155 ('mathtext.fallback_to_cm : True  # When True, use symbols from the Computer Modern')
You probably need to get an updated matplotlibrc file from
https://github.com/matplotlib/matplotlib/blob/v3.5.0/matplotlibrc.template
or from the matplotlib source distribution

Bad key savefig.jpeg_quality in file C:\ProgramData\Anaconda3\envs\cellprofiler\lib\site-packages\matplotlib\mpl-data\stylelib\_classic_test.mplstyle, line 418 ('savefig.jpeg_quality: 95       # when a jpeg is saved, the default quality parameter.')
You probably need to get an updated matplotlibrc file from
https://github.com/matplotlib/matplotlib/blob/v3.5.0/matplotlibrc.template
or from the matplotlib source distribution

Bad key keymap.all_axes in file C:\ProgramData\Anaconda3\envs\cellprofiler\lib\site-packages\matplotlib\mpl-data\stylelib\_classic_test.mplstyle, line 466 ('keymap.all_axes : a                 # enable all axes')
You probably need to get an updated matplotlibrc file from
https://github.com/matplotlib/matplotlib/blob/v3.5.0/matplotlibrc.template
or from the matplotlib source distribution

Bad key animation.avconv_path in file C:\ProgramData\Anaconda3\envs\cellprofiler\lib\site-packages\matplotlib\mpl-data\stylelib\_classic_test.mplstyle, line 477 ('animation.avconv_path: avconv     # Path to avconv binary. Without full path')
You probably need to get an updated matplotlibrc file from
https://github.com/matplotlib/matplotlib/blob/v3.5.0/matplotlibrc.template
or from the matplotlib source distribution

Bad key animation.avconv_args in file C:\ProgramData\Anaconda3\envs\cellprofiler\lib\site-packages\matplotlib\mpl-data\stylelib\_classic_test.mplstyle, line 479 ('animation.avconv_args:            # Additional arguments to pass to avconv')
You probably need to get an updated matplotlibrc file from
https://github.com/matplotlib/matplotlib/blob/v3.5.0/matplotlibrc.template
or from the matplotlib source distribution


## Omero Plugin

Error 1
Could not load loadimagesfromomero_SW
Traceback (most recent call last):
  File "c:\programdata\anaconda3\envs\cellprofiler\lib\site-packages\cellprofiler_core\utilities\core\modules\__init__.py", line 71, in add_module
    m = __import__(mod, globals(), locals(), ["__all__"], 0)
  File "C:\Users\MiN_Acc1\Documents\GitHub\CellProfiler_Omero\plugins\loadimagesfromomero_SW.py", line 48, in <module>
    from cellprofiler_core.modules import default_cpimage_name
ImportError: cannot import name 'default_cpimage_name' from partially initialized module 'cellprofiler_core.modules' (most likely due to a circular import) (c:\programdata\anaconda3\envs\cellprofiler\lib\site-packages\cellprofiler_core\modules\__init__.py)
- fixed line 48

Error 2
Traceback (most recent call last):
  File "c:\programdata\anaconda3\envs\cellprofiler\lib\site-packages\cellprofiler_core\utilities\core\modules\__init__.py", line 71, in add_module
    m = __import__(mod, globals(), locals(), ["__all__"], 0)
  File "C:\Users\MiN_Acc1\Documents\GitHub\CellProfiler_Omero\plugins\loadimagesfromomero_SW.py", line 148, in <module>
    M_C = "%s_%s" % (cpmeas.C_METADATA, FTR_C)
AttributeError: module 'cellprofiler_core.measurement' has no attribute 'C_METADATA'

Error 3
Traceback (most recent call last):
  File "c:\programdata\anaconda3\envs\cellprofiler\lib\site-packages\cellprofiler_core\utilities\core\modules\__init__.py", line 71, in add_module
    m = __import__(mod, globals(), locals(), ["__all__"], 0)
  File "C:\Users\MiN_Acc1\Documents\GitHub\CellProfiler_Omero\plugins\loadimagesfromomero_SW.py", line 772, in <module>
    class OmeroImageProvider(cpimage.AbstractImageProvider):
AttributeError: module 'cellprofiler_core.image' has no attribute 'AbstractImageProvider'

Error 4
Could not load loadimagesfromomero_SW
Traceback (most recent call last):
  File "c:\programdata\anaconda3\envs\cellprofiler\lib\site-packages\cellprofiler_core\utilities\core\modules\__init__.py", line 76, in add_module
    cp_module = find_cpmodule(m)
  File "c:\programdata\anaconda3\envs\cellprofiler\lib\site-packages\cellprofiler_core\utilities\core\modules\__init__.py", line 58, in find_cpmodule
    raise ValueError(
ValueError: Could not find cellprofiler_core.module.Module class in C:\Users\MiN_Acc1\Documents\GitHub\CellProfiler_Omero\plugins\loadimagesfromomero_SW.py



# New conda environment - cp_omero
(cp_omero) C:\Users\MiN_Acc1\Documents\GitHub\CellProfiler_Omero>cellprofiler
Failed to load LoadImagesFromOmero
Traceback (most recent call last):
  File "C:\Users\MiN_Acc1\AppData\Roaming\Python\Python38\site-packages\cellprofiler_core\utilities\core\modules\__init__.py", line 96, in add_module
    cp_module()
  File "C:\Users\MiN_Acc1\AppData\Roaming\Python\Python38\site-packages\cellprofiler_core\module\_module.py", line 88, in __init__
    self.create_settings()
  File "C:\Users\MiN_Acc1\Documents\GitHub\CellProfiler_Omero\plugins\loadimagesfromomero.py", line 194, in create_settings
    self.omero_host = cps.Text(
AttributeError: module 'cellprofiler_core.setting' has no attribute 'Text'
could not load these modules: loadimagesfromomero
