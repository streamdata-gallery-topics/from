---
swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 0
info:
  title: AWS Simple Email Service API Set Identity Mail From Domain
  version: 1.0.0
  description: Enables or disables the custom MAIL FROM domain setup for a verified
    identity (an email address or a domain).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetIdentityMailFromDomainAttributes:
    get:
      summary: Get Identity Mail From Domain Attributes
      description: Returns the custom MAIL FROM attributes for a list of identities
        (email addresses and/or domains).
      operationId: getIdentityMailFromDomainAttributes
      x-api-path-slug: actiongetidentitymailfromdomainattributes-get
      parameters:
      - in: query
        name: Identities.member.N
        description: A list of one or more identities
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=SetIdentityMailFromDomain:
    get:
      summary: Set Identity Mail From Domain
      description: Enables or disables the custom MAIL FROM domain setup for a verified
        identity (an email address or a domain).
      operationId: setIdentityMailFromDomain
      x-api-path-slug: actionsetidentitymailfromdomain-get
      parameters:
      - in: query
        name: BehaviorOnMXFailure
        description: The action that you want Amazon SES to take if it cannot successfully
          read the required MX record when you send an email
        type: string
      - in: query
        name: Identity
        description: The verified identity for which you want to enable or disable
          the specified custom MAIL FROM domain
        type: string
      - in: query
        name: MailFromDomain
        description: The custom MAIL FROM domain that you want the verified identity
          to use
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---