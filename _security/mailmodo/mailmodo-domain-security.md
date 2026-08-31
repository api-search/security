---
api_specs:
- filename: mailmodo-campaigns-api-openapi.yml
  format: yaml
  label: Mailmodo Campaigns API
  slug: mailmodo-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-campaigns-api-openapi.yml
- filename: mailmodo-contact-lists-api-openapi.yml
  format: yaml
  label: Mailmodo Contact Lists API
  slug: mailmodo-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-contact-lists-api-openapi.yml
- filename: mailmodo-contacts-api-openapi.yml
  format: yaml
  label: Mailmodo Contacts API
  slug: mailmodo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-contacts-api-openapi.yml
- filename: mailmodo-events-api-openapi.yml
  format: yaml
  label: Mailmodo Events API
  slug: mailmodo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-events-api-openapi.yml
- filename: mailmodo-templates-api-openapi.yml
  format: yaml
  label: Mailmodo Templates API
  slug: mailmodo-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-templates-api-openapi.yml
- filename: mailmodo-addevent-api-openapi.yml
  format: yaml
  label: Mailmodo Add Event API
  slug: mailmodo-addevent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-addevent-api-openapi.yml
- filename: mailmodo-addtolist-api-openapi.yml
  format: yaml
  label: Mailmodo Add To List API
  slug: mailmodo-addtolist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-addtolist-api-openapi.yml
- filename: mailmodo-bulktriggercampaign-api-openapi.yml
  format: yaml
  label: Mailmodo Bulktrigger Campaign API
  slug: mailmodo-bulktriggercampaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-bulktriggercampaign-api-openapi.yml
- filename: mailmodo-campaignreports-api-openapi.yml
  format: yaml
  label: Mailmodo Campaign Reports API
  slug: mailmodo-campaignreports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-campaignreports-api-openapi.yml
- filename: mailmodo-getallcontactlists-api-openapi.yml
  format: yaml
  label: Mailmodo Get All Contact Lists API
  slug: mailmodo-getallcontactlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-getallcontactlists-api-openapi.yml
- filename: mailmodo-getalltemplates-api-openapi.yml
  format: yaml
  label: Mailmodo Get All Templates API
  slug: mailmodo-getalltemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-getalltemplates-api-openapi.yml
- filename: mailmodo-getcontactdetails-api-openapi.yml
  format: yaml
  label: Mailmodo Get Contact Details API
  slug: mailmodo-getcontactdetails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-getcontactdetails-api-openapi.yml
- filename: mailmodo-hooks-api-openapi.yml
  format: yaml
  label: Mailmodo Hooks API
  slug: mailmodo-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-hooks-api-openapi.yml
- filename: mailmodo-removefromlist-api-openapi.yml
  format: yaml
  label: Mailmodo Remove From List API
  slug: mailmodo-removefromlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-removefromlist-api-openapi.yml
- filename: mailmodo-triggercampaign-api-openapi.yml
  format: yaml
  label: Mailmodo Trigger Campaign API
  slug: mailmodo-triggercampaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-triggercampaign-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mailmodo.com
  spf: true
hosts:
- cert_expires: Sep 21 21:48:54 2026 GMT
  host: www.mailmodo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: manage.mailmodo.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.mailmodo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailmodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailmodo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mailmodo
provider_slug: mailmodo
slug: mailmodo-domain-security
source_filename: mailmodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:48:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: manage.mailmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.mailmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mailmodo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/security/mailmodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Interactive Email
- AMP for Email
- Marketing Automation
- Transactional Email
- Campaigns
- Journeys
- Customer Engagement
---
