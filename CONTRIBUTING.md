# Contributing

Thanks for helping improve **Awesome GUI Agent**! Missing papers, broken links and updated venues are all welcome.

## How to contribute

1. Fork this repo and edit `README.md`, or open an issue with the paper link.
2. Put the paper in the matching section (Native Models / GUI Grounding / Agent Frameworks / World Models / RL / Data Synthesis / Safety / Benchmarks).
3. Within a section, use the right year block (publication year, or arXiv year for preprints) and keep the order **venue first, newest first**.
4. Use the formats below.

### Paper row (method sections)

```markdown
| ICLR<br><sup>2025</sup> | <sup>`ModelName`</sup> | Full Paper Title `Platform` <br> <sup><sub>*Author A, Author B, Author C, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/xxxx.xxxxx)\|[Code](https://github.com/owner/repo) |
```

- `Platform` is one of `Web`, `Mobile`, `Desktop`, `Windows`, `Cross-platform`, `Grounding` (or a combination such as `Web/Mobile`).
- If the paper introduces a dataset or benchmark, add a grey badge after the title:
  `<sub>![Name](https://img.shields.io/badge/Name-grey)</sub>`
- List at most 8 authors, then `et al.`
- Write a plain `Code` (no link) if the code has not been released.

### Benchmark row

```markdown
| **[Name](https://github.com/owner/repo)** | NeurIPS<br><sup>2024</sup> | Full Paper Title <br> <sup><sub>*Author A, Author B, et al.*</sub></sup> | [Paper](https://arxiv.org/abs/xxxx.xxxxx)\|[Code](https://github.com/owner/repo) |
```

## Checklist

- [ ] The paper is about GUI / computer-use agents (or a resource they directly depend on)
- [ ] Title, authors and venue match the official version
- [ ] Links open correctly
- [ ] The entry is not already in the list
