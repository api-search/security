---
api_specs:
- filename: anchore-images-api-openapi.yml
  format: yaml
  label: Anchore Images API
  slug: anchore-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-images-api-openapi.yml
- filename: anchore-policies-api-openapi.yml
  format: yaml
  label: Anchore Policies API
  slug: anchore-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-policies-api-openapi.yml
- filename: anchore-registries-api-openapi.yml
  format: yaml
  label: Anchore Registries API
  slug: anchore-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-registries-api-openapi.yml
- filename: anchore-sbom-api-openapi.yml
  format: yaml
  label: Anchore SBOM API
  slug: anchore-sbom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-sbom-api-openapi.yml
- filename: anchore-subscriptions-api-openapi.yml
  format: yaml
  label: Anchore Subscriptions API
  slug: anchore-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-subscriptions-api-openapi.yml
- filename: anchore-vulnerabilities-api-openapi.yml
  format: yaml
  label: Anchore Vulnerabilities API
  slug: anchore-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/openapi/anchore-vulnerabilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anchore.com
  spf: true
hosts:
- cert_expires: Aug 19 08:06:09 2026 GMT
  host: anchore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 08:06:09 2026 GMT
  host: docs.anchore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anchore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchore, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Anchore
provider_slug: anchore
slug: anchore-domain-security
source_filename: anchore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 08:06:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.anchore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 08:06:09 2026 GMT\n  hsts: false\ndomains:\n- domain: anchore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchore/refs/heads/main/security/anchore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Container Security
- Containers
- SBOM
- Software Supply Chain
- Vulnerability Scanning
---
