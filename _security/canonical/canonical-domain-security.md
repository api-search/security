---
api_specs:
- filename: rest-api.yaml
  format: yaml
  label: LXD REST API
  slug: lxd-api
  spec_type: OpenAPI
  url: https://github.com/canonical/lxd/blob/main/doc/rest-api.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:is-admin@canonical.com"
  - 0 issue "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: canonical.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:is-admin@canonical.com"
  - 0 issuewild "digicert.com"
  dmarc: false
  dnssec: false
  domain: snapcraft.io
  spf: true
hosts:
- cert_expires: Sep 30 04:13:37 2026 GMT
  host: canonical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.snapcraft.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.charmhub.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canonical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canonical, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Canonical
provider_slug: canonical
slug: canonical-domain-security
source_filename: canonical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canonical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:13:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.snapcraft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.charmhub.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: canonical.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:is-admin@canonical.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: snapcraft.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290\"\
  \n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:is-admin@canonical.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/security/canonical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Linux
- Open Source
- Ubuntu
- Containers
- Bare Metal
- Charms
- Identity
---
