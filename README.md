# LongInter Dataset

This is the repository for the paper:
> **LongInter: A Large and Diverse Benchmark for Long-term Human-Human Interactions**
> 
> [Hang Gao](https://www.linkedin.com/in/hang-gao-725986307/?originalSubdomain=au), [Zeyu Zhang](https://steve-zeyu-zhang.github.io), [Yuedong (Donny) Chen](https://donydchen.github.io/), Weiqiang Wang, Weijie Wang, Xiaolong Shen, [Jianfei Cai](https://jianfei-cai.github.io/)
> 
> ### [Paper]() | [LongInter Benchmark]()

## Citation

If you use any content of this repo for your work, please cite the following our paper:
```

```

## Introduction
Human-human interaction is fundamental to social behavior, with prolonged dyadic motions frequently observed in real-world scenarios such as dancing, sparring, and collaborative activities. These interactions are characterized by both long temporal duration, multi-stage and inter-person dependencies. However, existing datasets lack long-term dual-human sequences, and current 3D motion generation models struggle to capture long-range temporal dependencies in such settings.In this work, we present LongInter Benchmark: the first large-scale dataset focused on long-term human-human interactions. We collect high-quality 3D motion sequences by retrieving and transitioning existing short motions using retrieval-augmented generation and transition inference strategies. We apply rigorous filtering criteria to ensure motion realism and consistency. Additionally, we provide rich, extended textual annotations by summarizing short-sequence captions using large language models, resulting in a curated dataset of 7.7K interaction sequences and 9.8 million frames. To systematically evaluate the challenges and progress of this task, we first conduct performance benchmarking using representative SOTA models from short-sequence motion generation on our constructed dataset. Building upon the evaluation results, we design and introduce a new baseline model specifically tailored for modeling long-term, multi-stage human-human interactions.

## Demo Visualization

<table>
  <tr>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/b84df92e-ed92-4d17-82ae-1184c1aaefb8" width="500" height="500" controls></video><br>
      <b>Two individuals are dancing together, facing each other as they perform the social dance.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/4c70ea3d-69ec-4cee-934f-fb66583f8569" width="500" height="500" controls></video><br>
      <b>Two people are dancing together in a ballroom, practicing their dance moves as they enjoy the rhythm of the music.</b>
    </td>
        <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/e1f147ba-e4ee-401a-aed5-50575085451e" width="500" height="500" controls></video><br>
      <b>Two people are dancing together, performing a lively dance as one person learns the dance moves of the other. The two individuals are rehearsing Latin dance moves in unison.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/e18feda1-b400-4181-8295-f814f85e4258" width="500" height="500" controls></video><br>
      <b>Both of them kick with their left legs simultaneously and lift their right legs to kick one another. They then move forward and kick each other's legs, engaging in a kicking collision using their left legs.</b>
    </td>
  </tr>


  <tr>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/6c09fc6f-1fc0-4838-bf44-a71a8177e28c" width="500" height="500" controls></video><br>
      <b>One person steps forward, hugs the other person's shoulder, kisses him on the cheek, and the other person reciprocates by kissing him on the cheek and hugging him. Two people face each other and take turns stepping on each other's left foot with their right foot. Two people stand shoulder to shoulder, with one person placing his/her hand on the other person's shoulder, and then both of them extend their hands in a scissor pose. One person reaches out with both hands and assists the other person in standing up, while his legs rise.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/a5957665-9cef-4b1d-a7be-c8707d34c798" width="500" height="500" controls></video><br>
      <b>One person steps forward, hugs the other person's shoulder, kisses him on the cheek, and the other person reciprocates by kissing him on the cheek and hugging him. Then, one person walks closer to the other, who pushes him away with their right hand before stepping back. The first person sits, while the second person stands on his or her left side and uses both hands to massage his or her left shoulder. As one person sits still, they extend their left hand to hold the right hand of the standing person, who simultaneously bends his or her knees and lowers his or her body.</b>
    </td>
  <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/70f87045-52e2-4a98-8751-ab01ff63bde0" width="500" height="500" controls></video><br>
      <b>Two people stand face to face, with one person extending his or her hands and moving closer to cover the other person's mouth with his or her palms. The other person retreats a step. They then stand facing each other again, and the first person stretches out his or her right hand to touch the second person's head while the second person stands still. Next, they stand side by side, with one person holding the other's left arm with both hands and pulling him or her back, causing the other person to take a few steps while being pulled. Back in front of each other, the first person forcefully slaps the second person's face with his or her left and right hands, causing the second person to twist his or her body from side to side. Standing facing each other once more, one person extends his or her right hand and pulls the other person's right hand, pulling him or her forward. They then stand facing each other again, and the first person extends his or her left hand to pat the right cheek of the second person. Once more standing side by side, one person extends both hands to touch the shoulders of the other person as he or she walks forward slowly together. They stand facing each other again, with the first person placing his or her hands on the left ear of the second person and whispering. Finally, the second person extends his or her right hand above his or her head.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/cfcc7989-c5e9-47d0-b7db-ea809f0d003c" width="500" height="500" controls></video><br>
      <b>Two people stand face to face, with the first person extending his/her hands to grab the second person's right hand, pulling him/her towards the front. They continue to face each other as one person extends his/her right hand to grasp the left hand of the other and pulls him/her closer. Walking side by side, one person raises his/her right hand to grab the other person's left arm, moving forward together. Again, they stand facing each other, and the first person leans towards the second person, who also leans towards him/her. Standing face to face once more, one person extends his/her right foot and kicks the left shin of the other person, causing him/her to move sideways twice. Finally, with both still facing each other, the first person raises his/her right hand to lightly slap the right cheek of the second person.</b>
    </td>
  </tr>


  <tr>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/48f5b40c-ff2b-4f16-8ed5-2e222fce63a2" width="500" height="500" controls></video><br>
      <b>One person walks towards the other and places his or her right arm on the other person's shoulder, while the other person walks toward him or her and places his or her left hand on the first person's shoulder. They face each other as one person stretches out his or her right hand, directing the forefinger toward the other person. Subsequently, another gentleman approaches, extends both hands, and firmly clasps the man’s right hand. Both men stand, and one person extends his left hand, making a thumbs-down gesture toward the other person, who then extends his right hand and strikes him. They continue to stand facing each other until the first person takes a step forward, reaching out with both hands to grab the second person's left upper arm and leading him or her forward a few steps. One person holds the other person’s hand with his or her right hand while walking on his or her shoulder, as the other person jumps forward, holding the first person’s hand. Then, one person crouches down and carries him or her. The two people stand facing each other, with their right hands flat in front, their left hands gently beating their right hands, as they perform rock-paper-scissors three times. The first person raises his or her right hand, while the second person raises both hands. They clasp the right hand of the first person and shake it up and down in a handshake.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/0b7ce1b5-687c-4c69-92fd-aa20ccdd51ce" width="500" height="500" controls></video><br>
      <b>The two people almost bump into each other, and one person raises his hands to his chest and walks aside. One person covers the other person's right ear with both hands and whispers, while the other person covers his or her mouth with both hands. They then face each other, sit down, and twist their wrists with their right hands. Standing side by side and facing opposite directions, they wrap their right arms around each other's right arms and start spinning around, dancing together. Finally, they stand face to face, holding onto each other's arms and swaying back and forth, dancing.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/49523825-31f6-4aeb-8b11-d3607858fa58" width="500" height="500" controls></video><br>
      <b>Two people are standing, and one person rotates the other and kicks him on his left leg with their right leg. The first person sitting there extends his left hand, while the second person puts their right hand around the first person's left arm. They then stand up and walk forward together, facing each other with their right hands, swinging their hands from back to front and punching from bottom to top. They play three games of rock, paper, scissors. One person grabs his right arm with both hands and pulls, turning him to the right. The two people extend both hands to shake, and one person pulls the other person. The first person softly pats the upper left part of the second person's back from behind with his/her right hand. The standing person touches the head of the sitting person with his/her right hand, and the other person raises both hands.</b>
    </td>
    <td width="500" align="center" valign="top">
      <video src="https://github.com/user-attachments/assets/d46e494e-7a39-4cc7-a0eb-1d87ea9d3136" width="500" height="500" controls></video><br>
      <b>The first person stands in front of the second person, facing him, and gently kicks the second person's right calf with their right foot. Both people stand facing each other, communicating, as the first person occasionally waves his/her left hand up and down, while the second person waves his/her right hand in the same manner. An individual grasps the left hand of the other person, tugs him/her toward the front, and then the other individual proceeds to advance a few steps. One person stands to the left of the other, tiptoeing and raising both hands while whispering something to them. One person stretches out his/her hands to cover the other person's mouth, while simultaneously, the other person stretches out his/her right hand to cover the first person's mouth. The first person then leans back. One person slaps the other, but he/she does not react. Two people stand side by side, with the first person's right arm intertwined with the second person's left arm, and they walk forward together. One person walks to the left rear of the other person, who is sitting in a seat, and pats the right side of his/her back using his/her right hand. Two people stand side by side again, and one person embraces the other person's shoulder with his/her left hand and pats his/her cheek with the right hand, while the other person embraces this person's waist with his/her right hand.</b>
    </td>
  </tr>
</table>


## License

Our data is under NCND license. no commerical use. Do not modify our data for another dataset.

![license](https://github.com/user-attachments/assets/978cf963-0455-44fa-8027-c859af934753)























