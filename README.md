# 📈 Setup github actions 

## Job Artifacts and Outputs
- Jobs often produce assets that should be shared or analyzed.
- Examples: Deployable website files, logs, binaries etc.
- These assets are referred to as Artifacts or Job Artifacts.
- Github actions provides Actions for uploading and downloading these Artifacts.

## Caching
- Caching can help speed up repeated, slow Steps.
- Typical use case: Caching Dependencies.
- But any files and folders can be cached.
- The cache Action automatically stores and updates cache values based on the cache key.

## Outputs
- Besides Artifacts, Steps can produce and share simple values.
- These outputs are shared via ::set-output.
- Jobs can pick up and share Step outputs via the steps context.
- Other Jobs can use Job outputs via the needs cntext.
