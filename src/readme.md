A new and improved interactive interpreter, based on PyPy's, featuring multi-line editing and color support, as well as colorized exception tracebacks.
An experimental free-threaded build mode, which disables the Global Interpreter Lock, allowing threads to run more concurrently. The build mode is available as an experimental feature in the Windows and macOS installers as well.
A preliminary, experimental JIT, providing the ground work for significant performance improvements.
The locals() builtin function (and its C equivalent) now has well-defined semantics when mutating the returned mapping, which allows debuggers to operate more consistently.
A modified version of mimalloc is now included, optional but enabled by default if supported by the platform, and required for the free-threaded build mode.
Docstrings now have their leading indentation stripped, reducing memory use and the size of .pyc files. (Most tools handling docstrings already strip leading indentation.)
The dbm module has a new dbm.sqlite3 backend that is used by default when creating new files.
The minimum supported macOS version was changed from 10.9 to 10.13 (High Sierra). Older macOS versions will not be supported going forward.
WASI is now a Tier 2 supported platform. Emscripten is no longer an officially supported platform (but Pyodide continues to support Emscripten).
iOS is now a Tier 3 supported platform.
Android is now a Tier 3 supported platform.