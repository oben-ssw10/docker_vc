Due to the restricted license for data used in the paper, different model is trained for the voice conversion demo. We used 2 hours male speaker data from Hi-Fi Multi-Speaker English TTS Dataset (Hi-Fi TTS) [1].

[1] E. Bakhturina, "Hi-Fi Multi-Speaker English TTS Dataset", in Proceedings of Interspech, 2021, pp. 2776-2780.

Download the lpcnet demo: 

https://drive.google.com/file/d/1kj1SQgJOyJgantBRufkX6-DPVD491Yk_/view?usp=sharing

Pull the docker image:

docker pull oben2021/voice_conversion:demo

Please unzip the lpcnet_demo and run with the input wav file (16kHz):

sudo docker run --rm -it --init --volume="$PWD:/app" oben2020/voice_conversion:demo lpcnet_demo/convert.bin input.16k.wav
