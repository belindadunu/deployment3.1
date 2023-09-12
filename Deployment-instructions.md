<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>

## Deployment Instructions:
1. Create your own Jenkins Server and install the following on the server:
    - Install "python3.10-venv", "python-pip", "unzip", "[AWS CLI](https://scribehow.com/shared/How_to_Install_AWS_CLI__1MnhqmpcRxupkx_F-EcreQ)"
2. Create a multibranch pipeline and run the build for the application
3. Follow the install AWS EB CLI instructions
4. Then, add this stage to your Jenkins file and rerun your build: `stage (‘Deploy’) {
steps {
sh ‘eb deploy"
}
}
`
5. **IF** your application redeployed successfully, what did you notice?
6. **BONUS:** Once you've configured your webhook, change the background or some text in the application **HINT** Look into the HTML file and ask chatGPT
7. Did the application redeploy? 