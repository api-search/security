---
description: Domain security posture for the hosts NSwag is published from. The mechanical probe (0-working/probe-domain-security.py) returned "no-hosts" for this repo because every URL in apis.yml points at github.com, which the probe excludes as a platform host rather than a provider host. The probe below was therefore run by hand against nswag.org — the domain still declared as the project's homepage on the GitHub repository and printed in every published NuGet package — and the finding is that it no longer serves the project. Absence of records here is real recorded data, not a failed probe.
domains:
- caa: []
  caa_evidence: dig CAA nswag.org returned no records
  dmarc: false
  dmarc_evidence: dig TXT _dmarc.nswag.org returned no records
  dmarc_policy: null
  dnssec: false
  dnssec_evidence: dig DNSKEY nswag.org returned no records
  domain: nswag.org
  nameservers:
  - ns1.domaindiscount24.net.
  - ns2.domaindiscount24.net.
  - ns3.domaindiscount24.net.
  spf: false
  spf_evidence: dig TXT nswag.org returned no records
hosts:
- a_records:
  - 5.22.145.121
  - 5.22.145.16
  host: nswag.org
  hsts: null
  http_note: http://nswag.org/ returns 403 Forbidden with a text/html body and Cache-Control no-cache — a parked/denied host, not the project site.
  http_status: 403
  https: false
  https_error: TLS handshake timed out (443, 8s)
  resolved: true
  serving_project: false
- host: www.nswag.org
  hsts: null
  https: false
  https_error: TLS handshake timed out (443, 8s)
  serving_project: false
- host: github.com
  note: Platform host. NSwag's documentation (wiki), source, releases and issue tracker are all served by GitHub; GitHub's own TLS/HSTS/DNS posture is GitHub's, not NSwag's, and is deliberately not credited or debited here.
  probed: false
kind: domain-security
layout: security
method: probed
name: Nswag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NSwag, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NSwag
provider_slug: nswag
slug: nswag-domain-security
source_filename: nswag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: 'dig + TLS/HTTP probe, 2026-08-06'\ndescription: >-\n  Domain security posture for the hosts NSwag is published from. The mechanical\n  probe (0-working/probe-domain-security.py) returned \"no-hosts\" for this repo\n  because every URL in apis.yml points at github.com, which the probe excludes\n  as a platform host rather than a provider host. The probe below was therefore\n  run by hand against nswag.org — the domain still declared as the project's\n  homepage on the GitHub repository and printed in every published NuGet package\n  — and the finding is that it no longer serves the project. Absence of records\n  here is real recorded data, not a failed probe.\nhosts:\n  - host: nswag.org\n    https: false\n    https_error: 'TLS handshake timed out (443, 8s)'\n    http_status: 403\n    http_note: >-\n      http://nswag.org/ returns 403 Forbidden with a text/html body and\n      Cache-Control no-cache — a parked/denied host, not\
  \ the project site.\n    hsts: null\n    a_records: [5.22.145.121, 5.22.145.16]\n    resolved: true\n    serving_project: false\n  - host: www.nswag.org\n    https: false\n    https_error: 'TLS handshake timed out (443, 8s)'\n    hsts: null\n    serving_project: false\n  - host: github.com\n    probed: false\n    note: >-\n      Platform host. NSwag's documentation (wiki), source, releases and issue\n      tracker are all served by GitHub; GitHub's own TLS/HSTS/DNS posture is\n      GitHub's, not NSwag's, and is deliberately not credited or debited here.\ndomains:\n  - domain: nswag.org\n    dnssec: false\n    dnssec_evidence: 'dig DNSKEY nswag.org returned no records'\n    caa: []\n    caa_evidence: 'dig CAA nswag.org returned no records'\n    spf: false\n    spf_evidence: 'dig TXT nswag.org returned no records'\n    dmarc: false\n    dmarc_policy: null\n    dmarc_evidence: 'dig TXT _dmarc.nswag.org returned no records'\n    nameservers: [ns1.domaindiscount24.net., ns2.domaindiscount24.net.,\
  \ ns3.domaindiscount24.net.]\nfindings:\n  - severity: high\n    id: canonical-homepage-dead\n    detail: >-\n      NSwag.org is still the `homepage` field on github.com/RicoSuter/NSwag and\n      the project URL carried by every NuGet package, but it does not respond\n      over HTTPS and returns 403 over HTTP. Anyone following the link from a\n      package manager lands nowhere. The live documentation is the GitHub wiki\n      (https://github.com/RicoSuter/NSwag/wiki), which is what this catalog\n      records as Documentation.\n    remedy: >-\n      Either restore nswag.org or change the repository homepage and the package\n      PackageProjectUrl to the GitHub wiki, so the link a consumer follows from\n      NuGet resolves.\n  - severity: medium\n    id: no-email-authentication\n    detail: >-\n      nswag.org publishes neither SPF nor DMARC, so the domain is trivially\n      spoofable in mail claiming to come from the project.\n  - severity: low\n    id: no-dnssec-no-caa\n    detail:\
  \ 'No DNSKEY and no CAA records on nswag.org.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nswag/refs/heads/main/security/nswag-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- .NET
- ASP.NET Core
- C#
- Code Generation
- Developer Tools
- JSON-Schema
- Open-Source
- OpenAPI
- SDK
- Swagger
- TypeScript
---
