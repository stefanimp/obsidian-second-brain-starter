# Security and Privacy

This repository is a public starter kit. It should never contain private vault content, secrets, credentials, personal notes, or private links.

## Reporting Privacy Issues

If you find private data accidentally committed to this repository, open an issue with the minimum necessary context or contact the maintainer privately if contact information is available.

Do not repost sensitive content in public discussions.

## Scope

This repository contains Markdown templates and documentation. It does not include executable application code.

Security concerns are mostly related to accidental disclosure, such as:

- personal names or private relationships;
- local filesystem paths;
- access tokens or API keys;
- private URLs;
- screenshots with identifying information;
- copyrighted material copied from books, courses, or paid resources.

## Maintainer Checklist

Before every public release:

```bash
rg -n --hidden --glob '!**/.git/**' "token|password|api[_-]?key|secret|private key|C:\\Users|localhost|127\.0\.0\.1"
```

Also review all file names and attachments manually.
