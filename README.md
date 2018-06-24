# openfassNodeInfo
Openfaas application to print the container info



mkdir TestNodeInfo

faas-cli new test-node-info --lang node
find . | grep test-node-info

# Create handler.js, main.js, test-node-info.yaml package.json file in the same directory or download the files from the github

faas-cli build -f test-node-info.yml

faas-cli push -f test-node-info.yml

faas-cli deploy -f test-node-info.yml
