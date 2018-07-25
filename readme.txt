Requiremnt:
cpython2.7

How to use:
cpython2.7_dir/bin/python bytecode_profiler.py --trace target_program.py

Meta-options:
--help                Display this help then exit.
--version             Output version information then exit.
Otherwise, exactly one of the following three options must be given:
-t, --trace           Print python bytecode to sys.stdout before it is executed.
-b, --branch          Print branch infomation and hide bytecode
-r, --report          Generate a report from a counts file; do not execute
                      any code.  `--file' must specify the results file to
                      read, which must have been created in a previous run
                      with `--count --file=FILE'.
Modifiers:
-f, --file=<file>     File to accumulate counts over several runs.
-R, --no-report       Do not generate the coverage report files.
                      Useful if you want to accumulate over several runs.
-C, --coverdir=<dir>  Directory where the report files.  The coverage
                      report for <package>.<module> is written to file
                      <dir>/<package>/<module>.cover.
-m, --missing         Annotate executable lines that were not executed
, --summary         Write a brief summary on stdout for each file.
                      (Can only be used with --count or --report.)
-g, --timing          Prefix each line with the time since the program started.
                      Only used while tracing.
Filters, may be repeated multiple times:
--ignore-module=<mod> Ignore the given module(s) and its submodules
                      (if it is a package).  Accepts comma separated
                      list of module names
--ignore-dir=<dir>    Ignore files in the given directory (multiple
                      directories can be joined by os.pathsep).

