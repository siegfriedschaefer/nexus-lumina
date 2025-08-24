
gcloud auth application-default login

gcloud auth application-default set-quota-project $GCLOUD_PROJECT_NAME

## FAQ

When getting this error messages by running wavenet application:
------
  code: 2,
  details: 'Getting metadata from plugin failed with error: {"error":"invalid_grant","error_description":"reauth related error (invalid_rapt)","error_uri":"https://support.google.com/a/answer/9368756","error_subtype":"invalid_rapt"}',
  metadata: Metadata { internalRepr: Map(0) {}, options: {} },
  note: 'Exception occurred in retry method that was not classified as transient'
------

calling this google cloud console commande resolved the issue:
------
gcloud auth application-default login
------

