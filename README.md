# Dummy CMake project to test pre-commit hooks

## CMake execution
```
cmake -DCMAKE_BUILD_TYPE=Debug -B build
```

## pre-commit setup
```
pip install pre-commit
```

```
pre-commit install
```

## manual execution of pre-commit hooks
```
pre-commit run --all-files
```

## Example usage of clang-tidy-hook
This repository is configured to use [clang-tidy hook](https://github.com/mxmlnrdr/clang_tidy_hook) as code checker.  

See [GitHub Actions workflow](https://github.com/mxmlnrdr/dummy_repo/actions) for usage details.
* Ubuntu with gcc compiler
  -> clang-tidy hook prints warnings on terminal
* Ubuntu with clang compiler
    -> clang-tidy hook prints warnings on terminal
* Windows with Visual Studio compiler
    -> clang-tidy hook aborts as no compilation database available
