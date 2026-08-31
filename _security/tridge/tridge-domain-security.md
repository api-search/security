---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:re+houm4bhpeoi@dmarc.postmarkapp.com; sp=none; aspf=r;
  dnssec: false
  domain: tridge.com
  spf: true
  spf_record: v=spf1 include:_spf.mlsend.com a mx include:spf.mtasv.net  include:servers.mcsv.net include:_spf.google.com include:amazonses.com include:41698150.spf02.hubspotemail.net  ~all
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.tridge.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.tridge.com
  hsts: false
  https: true
  note: GraphQL surface host; root returns 404 and /graphql returns 403 "crc rejected" to anonymous callers.
  tls_version: TLSv1.2
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: accounts.tridge.com
  hsts: false
  https: true
  note: OAuth 2.0 authorization server host (/oauth/authorize, /oauth/token). No HSTS on an authentication host.
  tls_version: TLSv1.2
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: app.tridge.com
  hsts: false
  https: true
  note: Single-page web application; catch-all answers 200 text/html for every path.
  tls_version: TLSv1.2
- cert_expires: Nov  8 11:22:03 2026 GMT
  host: blog.tridge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: The only Tridge host observed serving HSTS, and the only one negotiating TLS 1.3 — it is externally hosted, not part of the core platform.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tridge, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tridge
provider_slug: tridge
slug: tridge-domain-security
source_filename: tridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Tridge host discovered during enrichment (apis.yml declares\n  no baseURL, so the extra hosts were probed by hand and are recorded with the same method)\nhosts:\n- host: www.tridge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.tridge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n  note: GraphQL surface host; root returns 404 and /graphql returns 403 \"crc rejected\" to anonymous callers.\n- host: accounts.tridge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n  note: OAuth 2.0 authorization server host (/oauth/authorize, /oauth/token). No HSTS on an authentication\n    host.\n- host: app.tridge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n  note: Single-page web application;\
  \ catch-all answers 200 text/html for every path.\n- host: blog.tridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 11:22:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: The only Tridge host observed serving HSTS, and the only one negotiating TLS 1.3 — it is externally\n    hosted, not part of the core platform.\ndomains:\n- domain: tridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.mlsend.com a mx include:spf.mtasv.net  include:servers.mcsv.net include:_spf.google.com\n    include:amazonses.com include:41698150.spf02.hubspotemail.net  ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:re+houm4bhpeoi@dmarc.postmarkapp.com; sp=none;\n    aspf=r;\nfindings:\n- No CAA record on tridge.com — any public CA may issue for the domain.\n- DNSSEC is not enabled on tridge.com.\n- No HSTS on www.tridge.com, api.tridge.com, accounts.tridge.com or app.tridge.com; the OAuth\
  \ authorization\n  host in particular carries no Strict-Transport-Security header.\n- Core platform hosts negotiate TLS 1.2 (not 1.3); only the externally hosted blog negotiates TLS 1.3.\n- SPF and DMARC are published; DMARC policy is p=quarantine with sp=none, so subdomains are not covered\n  by the parent policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tridge/refs/heads/main/security/tridge-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Agriculture
- Food
- Trade
- Commodities
- Market Data
- Supply Chain
- Sourcing
- Analytics
- Price Data
- Intelligence
- Artificial Intelligence
---
