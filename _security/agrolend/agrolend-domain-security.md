---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; sp=reject; rua=mailto:infra@agrolend.agr.br; adkim=s; aspf=s; pct=100; fo=1
  dnssec: false
  domain: agrolend.agr.br
  ds_records: []
  spf: true
  spf_record: v=spf1 include:_spf.google.com -all
hosts:
- cert_expires: '2026-11-15'
  cert_subject: CN=agrolend.agr.br
  host: agrolend.agr.br
  hsts: false
  hsts_max_age: null
  https: true
  note: 'The site root returns an infinite HTTP 301 self-redirect (Location: https://agrolend.agr.br/, x-redirect-by: WordPress), so the homepage is unreachable to any client that follows redirects. Interior pages (/quem-somos/, /relatorios/, /en/who-we-are/) serve 200 normally. /index.php/<slug>/ 301s to the internal origin hostname site-agrolend-639104121.us-east-1.elb.amazonaws.com, leaking the load balancer behind CloudFront.'
  role: marketing site (WordPress 6.7.7 behind CloudFront)
  tls_version: TLSv1.3
- cert_expires: '2026-10-08'
  cert_subject: CN=*.agrolend.agr.br
  host: parceiro.agrolend.agr.br
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'Answers HTTP 401 with WWW-Authenticate: Basic realm="Realm" on every path probed, including /.well-known/*, /openapi.json, /graphql and a negative-control path. /v3/api-docs, /v2/api-docs and /swagger-ui/* return 401 or 404 with no specification body, so springdoc is not exposed.'
  role: partner-area application backend (Spring Boot; JSON error envelope)
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: '2025-03-06'
  cert_subject: CN=*.agrolend.agr.br
  host: docs.agrolend.agr.br
  hsts: false
  http_status: 504
  https: true
  note: Resolves to agrolend-alb-dmz-apps-980323442.us-east-1.elb.amazonaws.com and serves a wildcard certificate that expired 2025-03-06; the load balancer returns 504 Gateway Time-out, so no backend is healthy. Dead infrastructure still holding a DNS name and an expired certificate.
  role: abandoned documentation host
  tls_version: TLSv1.2
- cert_expired: true
  cert_expires: '2025-03-06'
  cert_subject: CN=*.agrolend.agr.br
  host: portal.agrolend.agr.br
  hsts: false
  http_status: 504
  https: true
  note: Same dead ALB and same expired 2025-03-06 wildcard certificate as docs.agrolend.agr.br.
  role: abandoned portal host
  tls_version: TLSv1.2
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Agrolend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrolend, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agrolend
provider_slug: agrolend
slug: agrolend-domain-security
source_filename: agrolend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every agrolend.agr.br host discovered this pass\nnote: >-\n  Rewritten by hand after 0-working/probe-domain-security.py resolved the registrable domain to\n  \"agr.br\". \"agr.br\" is a Brazilian public suffix, not a registrable domain, so the script queried\n  the wrong zone and recorded spf:false / dmarc:false when agrolend.agr.br in fact publishes both\n  (DMARC p=reject). The registrable domain here is agrolend.agr.br. See the \"registrable domain\n  needs psl\" guardrail.\nhosts:\n- host: agrolend.agr.br\n  role: marketing site (WordPress 6.7.7 behind CloudFront)\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=agrolend.agr.br\n  cert_expires: '2026-11-15'\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    The site root returns an infinite HTTP 301 self-redirect (Location: https://agrolend.agr.br/,\n    x-redirect-by: WordPress), so the homepage is unreachable to any client that follows\
  \ redirects.\n    Interior pages (/quem-somos/, /relatorios/, /en/who-we-are/) serve 200 normally. /index.php/<slug>/\n    301s to the internal origin hostname site-agrolend-639104121.us-east-1.elb.amazonaws.com,\n    leaking the load balancer behind CloudFront.\n- host: parceiro.agrolend.agr.br\n  role: partner-area application backend (Spring Boot; JSON error envelope)\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=*.agrolend.agr.br\n  cert_expires: '2026-10-08'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Answers HTTP 401 with WWW-Authenticate: Basic realm=\"Realm\" on every path probed, including\n    /.well-known/*, /openapi.json, /graphql and a negative-control path. /v3/api-docs, /v2/api-docs\n    and /swagger-ui/* return 401 or 404 with no specification body, so springdoc is not exposed.\n- host: docs.agrolend.agr.br\n  role: abandoned documentation host\n  https: true\n  tls_version: TLSv1.2\n  cert_subject: CN=*.agrolend.agr.br\n\
  \  cert_expires: '2025-03-06'\n  cert_expired: true\n  hsts: false\n  http_status: 504\n  note: >-\n    Resolves to agrolend-alb-dmz-apps-980323442.us-east-1.elb.amazonaws.com and serves a wildcard\n    certificate that expired 2025-03-06; the load balancer returns 504 Gateway Time-out, so no\n    backend is healthy. Dead infrastructure still holding a DNS name and an expired certificate.\n- host: portal.agrolend.agr.br\n  role: abandoned portal host\n  https: true\n  tls_version: TLSv1.2\n  cert_subject: CN=*.agrolend.agr.br\n  cert_expires: '2025-03-06'\n  cert_expired: true\n  hsts: false\n  http_status: 504\n  note: Same dead ALB and same expired 2025-03-06 wildcard certificate as docs.agrolend.agr.br.\ndomains:\n- domain: agrolend.agr.br\n  dnssec: false\n  ds_records: []\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1; p=reject; sp=reject; rua=mailto:infra@agrolend.agr.br; adkim=s; aspf=s;\
  \ pct=100; fo=1\nfindings:\n- Email authentication is strong - SPF with a hard fail and DMARC p=reject with strict alignment.\n- No CAA records and no DNSSEC on the zone.\n- Two subdomains (docs, portal) serve certificates that expired eighteen months ago over TLS 1.2.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrolend/refs/heads/main/security/agrolend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Financial Services
- Lending
- Credit
- Fintech
- Brazil
- Rural Finance
- Banking
---
