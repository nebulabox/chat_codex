# Remote Repository File Handling

When given a public GitHub repository or file URL:

1. Open the exact URL directly; do not rely only on search-engine indexing.
2. Identify whether the URL is a repository, directory, blob, or raw-file URL.
3. Convert GitHub blob URLs to raw URLs automatically when binary content is needed.
4. Handle URL encoding for non-ASCII file names automatically.
5. Retrieve and verify the actual file content before claiming it was read.
6. Process the file according to its type: source code, image, PDF, archive, or binary.
7. Clearly distinguish between:
   - repository not found,
   - private repository,
   - page accessible but raw file unavailable,
   - file downloaded but unsupported,
   - content successfully retrieved.
8. Ask the user to upload the file only after reasonable direct-access methods have failed.
9. Never make the user perform URL conversion or file-location steps that can be completed automatically.

