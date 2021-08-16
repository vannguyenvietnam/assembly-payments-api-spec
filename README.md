# Generate Ruby SDK
## Install openapi-generator-cli
npm install @openapitools/openapi-generator-cli

## Generate SDK
npx openapi-generator-cli generate \
    -i ./swagger.yaml \
    -g ruby \
    -o ~/workspace/libs/assembly_payments_ruby/ \
    --additional-properties=gemName=assembly_ruby