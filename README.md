# Generate Ruby SDK
## Install openapi-generator-cli
npm install @openapitools/openapi-generator-cli

## Generate SDK
npx openapi-generator-cli generate \
    -i ./swagger.yaml \
    -g ruby \
    -o ~/workspace/libs/assembly_payments_ruby/ \
    --additional-properties=gemName=assembly_ruby

# Notes for custom endpoints:
## Add show batch transaction items
## Correct callbacks object_type enum values validation.
## Add limit and offset to show batch transaction and disbursement items.
## Add webhooks spec