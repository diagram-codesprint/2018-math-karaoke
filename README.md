# Math Karaoke

## Background Information

We will build a browser-based solution that display math equations and reads them aloud via text-to-speech with synchronized highlighting of the part being read, karaoke-style.

This will be an experimental approach and we'll iterate in search of a successful user experience. Educators and students with experience with dyslexia could provide valuable feedback and guide the approach of the project.

The project doesn't have to involve very advanced math, so no worries if you’re not a math wiz :slightly_smiling_face:

This would also be an opportunity to experiment with higher quality text-to-speech reading of math equations, including control of prosody (pause, volume, pitch, intensity) using SSML (if you're into that sort of thing).

At the end of the project, we will have authored some simple content (tutorial on solving quadratic equations?) that will be easier for dyslexic students to access.



## Setup
This demo uses the Amazon Polly text-to-speech synthesizer.
To use it, you need AWS credentials (API keys), which can be obtained on the AWS
console.
Store them in a file called keys.js with the following format
```javascript
if (window.AWS) {
    AWS.config.region = 'eu-west-1';
    AWS.config.accessKeyId = '<YOUR-KEY>';
    AWS.config.secretAccessKey = '<YOUR-SECRET>';
}
```
