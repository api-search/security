---
api_specs:
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Repositories API
  slug: gitee-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Issues API
  slug: gitee-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Pull Requests API
  slug: gitee-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Users and Organizations API
  slug: gitee-users-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Gists API
  slug: gitee-gists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Enterprises API
  slug: gitee-enterprises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Webhooks API
  slug: gitee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
description: ''
domains:
- a_records:
  - 180.76.199.13
  - 180.76.198.225
  caa: []
  caa_note: No CAA records returned.
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1;p=quarantine;pct=50;rua=mailto:liminghua@oschina.cn;ruf=mailto:liminghua@oschina.cn
  dnssec: false
  domain: gitee.com
  spf: true
  spf_record: v=spf1 include:spf.qiye.aliyun.com -all
hosts:
- cert_expires: Feb 20 06:59:59 2027 GMT
  cert_issuer: TrustAsia DV TLS RSA CA 2024
  cert_not_before: Jan 29 07:00:00 2026 GMT
  cipher: TLS_AES_256_GCM_SHA384
  host: gitee.com
  hsts: false
  hsts_note: No Strict-Transport-Security header was observed on the gitee.com root response.
  https: true
  ratelimit_header: true
  ratelimit_limit: 60
  ratelimit_note: X-RateLimit-Limit 60 observed on GET /api/v5/repos/oschina/git-osc (unauthenticated).
  server: ADAS/1.0.214
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gitee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gitee
provider_slug: gitee
slug: gitee-domain-security
source_filename: gitee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gitee.com\n  https: true\n  tls_version: TLSv1.3\n  cipher: TLS_AES_256_GCM_SHA384\n  cert_issuer: TrustAsia DV TLS RSA CA 2024\n  cert_not_before: Jan 29 07:00:00 2026 GMT\n  cert_expires: Feb 20 06:59:59 2027 GMT\n  hsts: false\n  hsts_note: No Strict-Transport-Security header was observed on the gitee.com root response.\n  server: ADAS/1.0.214\n  ratelimit_header: true\n  ratelimit_limit: 60\n  ratelimit_note: X-RateLimit-Limit 60 observed on GET /api/v5/repos/oschina/git-osc (unauthenticated).\ndomains:\n- domain: gitee.com\n  dnssec: false\n  caa: []\n  caa_note: No CAA records returned.\n  spf: true\n  spf_record: v=spf1 include:spf.qiye.aliyun.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1;p=quarantine;pct=50;rua=mailto:liminghua@oschina.cn;ruf=mailto:liminghua@oschina.cn\n  a_records:\n  - 180.76.199.13\n  - 180.76.198.225\n\
  notes: >-\n  gitee.com serves the site and the Open API v5 from the same host over TLS 1.3\n  with a TrustAsia DV certificate. HSTS was not present on the probed root\n  response. Email domain policy is present (SPF hard-fail via Aliyun; DMARC\n  quarantine at 50%). Gitee is operated from mainland China and is\n  ICP-registered; DNS resolves to Baidu-hosted infrastructure (180.76.x.x).\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/security/gitee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Code Hosting
- Git
- Git Hosting
- Version Control
- Repositories
- Pull Requests
- Issue Tracking
- DevOps
- Open Source
- China
---
