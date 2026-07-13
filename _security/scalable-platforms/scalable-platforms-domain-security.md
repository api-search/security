---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Vercel REST API
  slug: vercel-rest-api
  spec_type: OpenAPI
  url: https://openapi.vercel.sh/
- filename: openapi.yaml
  format: yaml
  label: Netlify API
  slug: netlify-api
  spec_type: OpenAPI
  url: https://open-api.netlify.com/
- filename: openapi.yaml
  format: yaml
  label: Cloudflare API
  slug: cloudflare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/cloudflare/api-schemas/main/openapi.yaml
- filename: api-docs
  format: yaml
  label: Heroku Platform API
  slug: heroku-platform-api
  spec_type: OpenAPI
  url: https://devcenter.heroku.com/api-docs
- filename: openapi.yaml
  format: yaml
  label: Fly.io Machines API
  slug: flyio-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/superfly/fly-openapi/refs/heads/main/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Render API
  slug: render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/renderinc/openapi-specs/main/openapi.yaml
- filename: openapi.json
  format: json
  label: Northflank API
  slug: northflank-api
  spec_type: OpenAPI
  url: https://api.northflank.com/v1/openapi.json
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vercel.com
  spf: true
hosts:
- cert_expires: Aug 21 08:55:49 2026 GMT
  host: api.vercel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalable Platforms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalable Platforms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalable Platforms
provider_slug: scalable-platforms
slug: scalable-platforms-domain-security
source_filename: scalable-platforms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.vercel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 08:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vercel.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/security/scalable-platforms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
---
