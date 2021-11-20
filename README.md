Download the lpcnet demo: 

https://drive.google.com/file/d/1kj1SQgJOyJgantBRufkX6-DPVD491Yk_/view?usp=sharing

Pull the docker image:

```docker pull oben2020/voice_conversion:demo

Please unzip the lpcnet_demo and run with the input wav file (16bits 16kHz mono):

```sudo docker run --rm -it --init --volume="$PWD:/app" oben2020/voice_conversion:demo lpcnet_demo/convert.bin input.16k.wav

# Disclaimer
Due to the restricted license of data used in the paper, a different model is trained for this voice conversion demo. We used 2 hours data (Reader 9017) from Hi-Fi TTS [1] as a target speaker.

[1] E. Bakhturina, "Hi-Fi Multi-Speaker English TTS Dataset", in Proceedings of Interspech, 2021, pp. 2776-2780.

# License
The pre-trained models are under the Create Commons Attribution-NonCommercial-ShareAlike-3.0 Unported (CC-BY-NC-SA 3.0) License.
