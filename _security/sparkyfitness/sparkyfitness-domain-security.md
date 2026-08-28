---
api_specs:
- filename: sparkyfitness-openapi.yml
  format: yaml
  label: SparkyFitness API
  slug: sparkyfitness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkyfitness/refs/heads/main/openapi/sparkyfitness-openapi.yml
description: ''
domains: []
hosts:
- attribution: infrastructure-provider
  host: codewithcj.github.io
  hsts:
    include_subdomains: false
    max_age: 31556952
    note: Set by GitHub Pages for all Pages sites.
    preload: false
    present: true
  https:
    certificate:
      issuer: Let's Encrypt (CN=YR1)
      not_after: '2026-10-31'
      not_before: '2026-08-02'
      note: Shared wildcard certificate covering every GitHub Pages user site.
      subject: CN=*.github.io
    reachable: true
    status: 200
    tls_protocol: TLSv1.3
  owner: GitHub (shared Pages wildcard) — not SparkyFitness
  server_header: GitHub.com
kind: domain-security
layout: security
method: probed
name: Sparkyfitness Domain Security
name_suffix: Domain Security
overview: Domain security posture for SparkyFitness, probed live across 1 host(s) and 0 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS.
provider_name: SparkyFitness
provider_slug: sparkyfitness
slug: sparkyfitness-domain-security
source_filename: sparkyfitness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: probed 2026-08-27 against https://codewithcj.github.io/SparkyFitness/\nfinding: >-\n  SparkyFitness controls no domain of its own. There is no vendor API host to\n  probe (the product is self-hosted, so every API host belongs to an operator)\n  and the only surface the project publishes is a GitHub Pages site under\n  codewithcj.github.io. The automated pipeline probe returned `no-hosts` for\n  exactly this reason — pipeline_util.provider_hosts deliberately excludes\n  github.io, because the TLS, HSTS and DNS posture of a Pages host measures\n  GitHub's infrastructure, not the project's. The results below are recorded\n  with that attribution made explicit, and MUST NOT be read as a security\n  posture SparkyFitness chose or maintains.\nprovider_controlled_domain: null\nhosts:\n  - host: codewithcj.github.io\n    owner: GitHub (shared Pages wildcard) — not SparkyFitness\n    attribution: infrastructure-provider\n    https:\n\
  \      reachable: true\n      status: 200\n      tls_protocol: TLSv1.3\n      certificate:\n        subject: CN=*.github.io\n        issuer: \"Let's Encrypt (CN=YR1)\"\n        not_before: '2026-08-02'\n        not_after: '2026-10-31'\n        note: Shared wildcard certificate covering every GitHub Pages user site.\n    hsts:\n      present: true\n      max_age: 31556952\n      include_subdomains: false\n      preload: false\n      note: Set by GitHub Pages for all Pages sites.\n    server_header: GitHub.com\ndns:\n  registrable_domain: github.io\n  attribution: >-\n    github.io is GitHub's domain. These records are GitHub's and are recorded\n    only to make clear what was and was not observable.\n  dnssec:\n    dnskey_present: false\n    note: No DNSKEY returned for github.io.\n  caa:\n    present: true\n    records:\n      - '0 issuewild \"sectigo.com\"'\n      - '0 issue \"digicert.com\"'\n      - '0 issue \"letsencrypt.org\"'\n  spf:\n    present: true\n    record: v=spf1 a -all\n\
  \  dmarc:\n    present: false\n    note: No TXT record at _dmarc.github.io.\ninterpretation: >-\n  For a self-hosted product the domain-security dimension is genuinely not the\n  project's to answer, and scoring it as a gap would misattribute GitHub's\n  configuration to SparkyFitness. What IS the project's to answer, and what it\n  does answer, is the security posture of the software an operator deploys:\n  PostgreSQL row-level security on every user-scoped read, admin-gated\n  developer tools that are off by default, MFA with an admin mandatory-MFA\n  switch, WebAuthn passkeys, OIDC federation, nginx rate limiting on every\n  authentication endpoint, and per-API-key rate limits. Those are recorded in\n  authentication/sparkyfitness-authentication.yml and\n  rate-limits/sparkyfitness-rate-limits.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparkyfitness/refs/heads/main/security/sparkyfitness-domain-security.yml
summary_line: HSTS
tags:
- Company
- Health
- Fitness
- Nutrition
- Self-Hosted
- Open Source
- Wearables
- MCP
- AI Assistant
- Quantified Self
---
