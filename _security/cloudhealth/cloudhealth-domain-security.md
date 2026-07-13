---
api_specs:
- filename: cloudhealth-openapi.yml
  format: yaml
  label: CloudHealth REST API
  slug: cloudhealth-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/openapi/cloudhealth-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vmware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudhealthtech.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: apidocs.cloudhealthtech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: chapi.cloudhealthtech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cloudhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudHealth, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CloudHealth
provider_slug: cloudhealth
slug: cloudhealth-domain-security
source_filename: cloudhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vmware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.cloudhealthtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: chapi.cloudhealthtech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vmware.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cloudhealthtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudhealth/refs/heads/main/security/cloudhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Cost
- Cloud Governance
- Cloud Management
- Cost Optimization
- FinOps
- Multi-Cloud
---
