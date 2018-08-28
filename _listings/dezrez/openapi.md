swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/metadata/{major}/{minor}/{build}/{revision}:
    get:
      summary: Returns the data contract to configure the word plugin for creating
        templates
      description: Returns the data contract to configure the word plugin for creating
        templates.
      operationId: DocumentGeneration_GetLetterEditorDataContractBymajorByminorBybuildByrevision
      x-api-path-slug: apidocumentgenerationmetadatamajorminorbuildrevision-get
      parameters:
      - in: path
        name: build
      - in: path
        name: major
      - in: path
        name: minor
      - in: path
        name: revision
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Data
      - Contract
      - To
      - Configure
      - Word
      - Plugincreating
      - Templates
  /api/documentgeneration/unusedmergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency that are
        not currently used in any envelope templates
      description: Returns a list of lettertemplates associated to this agency that
        are not currently used in any envelope templates.
      operationId: DocumentGeneration_GetUnusedMergeTemplates
      x-api-path-slug: apidocumentgenerationunusedmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - That
      - Are
      - Not
      - Currently
      - Used
      - In
      - Any
      - Envelope
      - Templates
  /api/documentgeneration/insertabletemplates:
    get:
      summary: Returns a list of insertable templates associated to this agency
      description: Returns a list of insertable templates associated to this agency.
      operationId: DocumentGeneration_GetPrintableInsertableTemplates
      x-api-path-slug: apidocumentgenerationinsertabletemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Insertable
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/documentgeneration/envelopetemplates:
    get:
      summary: Returns a list of envelope templates associated to this agency
      description: Returns a list of envelope templates associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplates
      x-api-path-slug: apidocumentgenerationenvelopetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/emailtemplates:
    get:
      summary: Returns a list of email templates associated to this agency
      description: Returns a list of email templates associated to this agency.
      operationId: DocumentGeneration_GetEmailTemplates
      x-api-path-slug: apidocumentgenerationemailtemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Email
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/smstemplates:
    get:
      summary: Returns a list of sms templates associated to this agency
      description: Returns a list of sms templates associated to this agency.
      operationId: DocumentGeneration_GetSmsTemplates
      x-api-path-slug: apidocumentgenerationsmstemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Sms
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/branding/uploadsmstemplate:
    post:
      summary: Upload the data to create a SMS Document Template for a Brand.
      description: Upload the data to create a sms document template for a brand..
      operationId: Branding_UploadSMSTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploadsmstemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - SMS
      - Document
      - Templatea
      - Brand
  /api/branding/uploademailtemplate:
    post:
      summary: Upload the data to create a Email Document Template for a Brand.
      description: Upload the data to create a email document template for a brand..
      operationId: Branding_UploadEmailTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploademailtemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - Email
      - Document
      - Templatea
      - Brand
  /api/documentgeneration/saveenvelopetemplate:
    post:
      summary: Saves or updates the envelope template for an agency
      description: Saves or updates the envelope template for an agency.
      operationId: DocumentGeneration_SaveEnvelopeTemplateByenvelopeTemplate
      x-api-path-slug: apidocumentgenerationsaveenvelopetemplate-post
      parameters:
      - in: body
        name: envelopeTemplate
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Updates
      - Envelope
      - Templatean
      - Agency
  /api/documentgeneration/templates/{templateType}:
    get:
      summary: Returns a list of mergable templates for any type associated to this
        agency
      description: Returns a list of mergable templates for any type associated to
        this agency.
      operationId: DocumentGeneration_GetTemplatesBytemplateType
      x-api-path-slug: apidocumentgenerationtemplatestemplatetype-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: templateType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Mergable
      - Templatesany
      - Type
      - Associated
      - To
      - This
      - Agency