This is the demo page for the paper **"KARASINGER: SCORE-FREE SINGING VOICE SYNTHESIS WITH VQ-VAE USING MEL-SPECTROGRAMS"**


## Abstract
In this paper, we propose a novel neural network model called KaraSinger for a less-studied singing voice synthesis (SVS) task named score-free SVS, in which the prosody and melody are spontaneously decided by machine. KaraSinger comprises a vector-quantized variational autoencoder (VQ-VAE) that compresses the Mel-spectrograms of singing audio to sequences of discrete codes, and a language model (LM) that learns to predict the discrete codes given the corresponding lyrics. For the VQ-VAE part, we employ a Connectionist Temporal Classification (CTC) loss to encourage the discrete codes to carry phoneme-related information. For the LM part, we use location-sensitive attention for learning a robust alignment between the input phoneme sequence and the output discrete code. We keep the architecture of both the VQ-VAE and LM light-weight for fast training and inference speed. We validate the effectiveness of the proposed design choices using a proprietary collection of 550 English pop songs sung by multiple amateur singers. The result of a listening test shows that KaraSinger achieves high scores in intelligibility, musicality, and the overall quality.

<hr>

### Audio Samples

We provide short samples from the subjective evalutaion described in the paper and long-length samples.


#### Short samples
Lyrics:
1. Just a small town girl living in a lonely world
2. She took the midnight train going anywhere
3. It goes on and on and on and on
4. She's got a smile that it seems to me
5. Take a sad song and make it better

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>KaraSinger</td>
      <td>3-level</td>
      <td>noCTC</td>
    </tr>
    <tr>
      <td>Sample 1</td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/proposed/0.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/3level/0.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/noctc/0.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 2</td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/proposed/1.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/3level/1.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/noctc/1.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 3</td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/proposed/2.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/3level/2.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/noctc/2.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 4</td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/proposed/3.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/3level/3.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/noctc/3.wav" type="audio/wav" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sample 5</td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/proposed/4.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/3level/4.wav" type="audio/wav" /></audio></td>
      <td><audio controls="" style="width: 160px;height: 50px"><source src="./assets/audios/noctc/4.wav" type="audio/wav" /></audio></td>
    </tr>
  </tfoot>
</table>

<hr>

#### Long samples with accompaniments

Lyrics: \
In this paper we propose \
a novel neural network model \
called Karaoke singer for a less studied \
singing voice synthesis task \
named score-free SVS \
in which the prosody and melody are spontaneously decided by machine.

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>KaraSinger</td>
    </tr>
    <tr>
      <td>Sample 1</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics1/temp0.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 2</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics1/temp1.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 3</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics1/temp2.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 4</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics1/temp3.wav" type="audio/wav" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sample 5</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics1/temp4.wav" type="audio/wav" /></audio></td>
    </tr>
  </tfoot>
</table>

Lyrics: \
台灣人工智慧實驗室 (Taiwan AI labs) \
is a privately funded \
research organization based in Taipei. \
Our goal is to leverage \
unique advantages in Taiwan \
to build AI solutions \
to solve the worlds problems.

<table style='text-align: center;'>
  <tbody>
    <tr>
      <td></td>
      <td>KaraSinger</td>
    </tr>
    <tr>
      <td>Sample 1</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics2/temp0.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 2</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics2/temp1.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 3</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics2/temp2.wav" type="audio/wav" /></audio></td>
    </tr>
    <tr>
      <td>Sample 4</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics2/temp3.wav" type="audio/wav" /></audio></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sample 5</td>
      <td><audio controls=""><source src="./assets/audios/long/lyrics2/temp4.wav" type="audio/wav" /></audio></td>
    </tr>
  </tfoot>
</table>

<hr>

### Contact 
Chien-Feng Liao: jerrygood0703@gmail.com

This project is developed and supported by <a href="https://ailabs.tw/about-us">Taiwan AI Labs</a>

