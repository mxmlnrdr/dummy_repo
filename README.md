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
