---
api_specs:
- filename: interpublic-wp-v2-api-openapi.yml
  format: yaml
  label: Interpublic Group WordPress Wp/v2 API
  slug: wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-wp-v2-api-openapi.yml
- filename: interpublic-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Interpublic Group WordPress Abilities API
  slug: wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-wp-abilities-v1-api-openapi.yml
- filename: interpublic-oembed-1-0-api-openapi.yml
  format: yaml
  label: Interpublic Group oEmbed API
  slug: oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-oembed-1-0-api-openapi.yml
- filename: interpublic-root-api-openapi.yml
  format: yaml
  label: Interpublic Group WordPress REST Index API
  slug: root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/openapi/interpublic-root-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: interpublic.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 28 10:57:05 2026 GMT
  host: www.interpublic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:02:27 2026 GMT
  host: interpublic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interpublic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interpublic Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Interpublic Group
provider_slug: interpublic
slug: interpublic-domain-security
source_filename: interpublic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interpublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:57:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\n- host: interpublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: interpublic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interpublic/refs/heads/main/security/interpublic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Marketing
- Fortune 500
- Holding Company
- Media
- Content
- WordPress
- Newsroom
---
