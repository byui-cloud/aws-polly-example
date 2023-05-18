# aws-polly-example
Pyhton example of getting user to enter text, send it to AWS Polly, and get Audio file back.

Need to do two pip (packages) installs with admin/su rights.

* pip3 install boto3
* python -m pip install pysimplegui

API Document https://docs.aws.amazon.com/polly/latest/dg/API_SynthesizeSpeech.html

CLI:

https://docs.aws.amazon.com/polly/latest/dg/get-started-cli-exercise.html

Get list of voices:
aws polly describe-voices --language-code en-US

Get mp3 audio:
aws polly synthesize-speech --output-format mp3 --voice-id Joanna --text 'Hello, my name is Super Student. I learned about AWS on April of 2023.' hello_aws.mp3


