swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 1
info:
  title: SalesLoft
  description: salesloft-helps-transform-sales-teams-into-modern-sales-organizations---converting-more-target-accounts-into-customer-accounts
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/email_templates.json:
    get:
      summary: List email templates
      description: |-
        Fetches multiple email template records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.email_templates.json.get
      x-api-path-slug: v2email-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of email templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: linked_to_team_template
        description: Filters email templates by whether they are linked to a team
          template or not
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Email
      - Templates
  /v2/team_templates.json:
    get:
      summary: List team templates
      description: |-
        Fetches multiple team template records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Team templates are templates that are available team-wide. Admins may use
        team templates to create original content for the entire team, monitor version control to ensure templates are always up to date,
        and track template performance across the entire organization. All metrics on a team template reflect usage across the team; individual metrics can be found with the email_templates API endpoint.
      operationId: v2.team_templates.json.get
      x-api-path-slug: v2team-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of team templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Team
      - Templates