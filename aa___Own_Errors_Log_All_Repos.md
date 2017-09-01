# Logging all kinds of errors - specially package installs etc 

#

01 sep 17 -- From PyPi while getting - distribute-0.7.3.zip , as a dependency for "slate" PDF Parser module for Py

```

dhankar@dhankar-VPCEB44EN:~$ pip install PyPDF2
Collecting PyPDF2
  Downloading PyPDF2-1.26.0.tar.gz (77kB)
    100% |████████████████████████████████| 81kB 142kB/s 
Building wheels for collected packages: PyPDF2
  Running setup.py bdist_wheel for PyPDF2 ... done
  Stored in directory: /home/dhankar/.cache/pip/wheels/86/6a/6a/1ce004a5996894d33d93e1fb1b67c30973dc945cc5875a1dd0
Successfully built PyPDF2
Installing collected packages: PyPDF2
Successfully installed PyPDF2-1.26.0
dhankar@dhankar-VPCEB44EN:~$ pip install slate
Collecting slate
  Downloading slate-0.3.zip
Collecting distribute (from slate)
  Downloading distribute-0.7.3.zip (145kB)
    100% |████████████████████████████████| 153kB 479kB/s 
    Complete output from command python setup.py egg_info:
    running egg_info
    creating pip-egg-info/distribute.egg-info
    writing requirements to pip-egg-info/distribute.egg-info/requires.txt
    writing pip-egg-info/distribute.egg-info/PKG-INFO
    writing top-level names to pip-egg-info/distribute.egg-info/top_level.txt
    writing dependency_links to pip-egg-info/distribute.egg-info/dependency_links.txt
    Traceback (most recent call last):
      File "<string>", line 1, in <module>
      File "/tmp/pip-build-7toJMU/distribute/setup.py", line 58, in <module>
        setuptools.setup(**setup_params)
      File "/home/dhankar/anaconda2/lib/python2.7/distutils/core.py", line 151, in setup
        dist.run_commands()
      File "/home/dhankar/anaconda2/lib/python2.7/distutils/dist.py", line 953, in run_commands
        self.run_command(cmd)
      File "/home/dhankar/anaconda2/lib/python2.7/distutils/dist.py", line 972, in run_command
        cmd_obj.run()
      File "setuptools/command/egg_info.py", line 177, in run
        writer = ep.load(installer=installer)
      File "pkg_resources.py", line 2241, in load
        if require: self.require(env, installer)
      File "pkg_resources.py", line 2254, in require
        working_set.resolve(self.dist.requires(self.extras),env,installer)))
      File "pkg_resources.py", line 2471, in requires
        dm = self._dep_map
      File "pkg_resources.py", line 2682, in _dep_map
        self.__dep_map = self._compute_dependencies()
      File "pkg_resources.py", line 2699, in _compute_dependencies
        from _markerlib import compile as compile_marker
    ImportError: No module named _markerlib
    
    ----------------------------------------
Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-build-7toJMU/distribute/
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ easy_install distribute
Searching for distribute
Reading https://pypi.python.org/simple/distribute/
Downloading https://pypi.python.org/packages/5f/ad/1fde06877a8d7d5c9b60eff7de2d452f639916ae1d48f0b8f97bf97e570a/distribute-0.7.3.zip#md5=c6c59594a7b180af57af8a0cc0cf5b4a
Best match: distribute 0.7.3
Processing distribute-0.7.3.zip
Writing /tmp/easy_install-mvScwN/distribute-0.7.3/setup.cfg
Running distribute-0.7.3/setup.py -q bdist_egg --dist-dir /tmp/easy_install-mvScwN/distribute-0.7.3/egg-dist-tmp-Lb2Z4A
warning: install_lib: 'build/lib' does not exist -- no Python modules to install

Moving distribute-0.7.3-py2.7.egg to /home/dhankar/anaconda2/lib/python2.7/site-packages
Adding distribute 0.7.3 to easy-install.pth file

Installed /home/dhankar/anaconda2/lib/python2.7/site-packages/distribute-0.7.3-py2.7.egg
Processing dependencies for distribute
Finished processing dependencies for distribute
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ pip install slate
Collecting slate
  Using cached slate-0.3.zip
Requirement already satisfied: distribute in ./anaconda2/lib/python2.7/site-packages/distribute-0.7.3-py2.7.egg (from slate)
Requirement already satisfied: setuptools>=0.7 in ./anaconda2/lib/python2.7/site-packages/setuptools-27.2.0-py2.7.egg (from distribute->slate)
Building wheels for collected packages: slate
  Running setup.py bdist_wheel for slate ... done
  Stored in directory: /home/dhankar/.cache/pip/wheels/1e/fa/10/b213e660eb6631216ed5aa6f3a8fb599c9d059ab1402053e95
Successfully built slate
Installing collected packages: slate
Successfully installed slate-0.3
dhankar@dhankar-VPCEB44EN:~$ 
dhankar@dhankar-VPCEB44EN:~$ 


```

#



#



#
