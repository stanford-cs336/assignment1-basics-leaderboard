# CS336 Spring 2025 Assignment 1 (Basics) Leaderboard

> [!NOTE]
> If you're a non-Stanford student and interested in submitting to the leaderboard, please create a pull request adding your result to the **second** table. To remain in the top 5, your submission must be verified, for which you should invite `marcelroed` to a minimal repo containing a uv project with `pyproject.toml`, `uv.lock` and `main.py`. Your script should be able to be reproduced on a single H100 by running `uv run main.py`.

To submit to the leaderboard, submit a pull request that adds your results to the Markdown table below. The table should be sorted by increasing loss.

Note that your submission can run for at most 1.5 hours on an H100, and that you may only use the OpenWebText training dataset that we provide.
The code must clearly be your own work, and you can't use external implementations for systems-critical aspects of your model.

The top 3 submissions will receive a prize at the end of the quarter, and the external top 3 submissions will receive a T-shirt.
To make this fair, we will reorder the top 5 scoring students based on our reproduced training runs.
**Make sure you save a snapshot of your best code so it can be reproduced by us!**
We will reach out to the top few students after results have stabilized.
Leading submissions that cannot be verified will be removed.

In your pull request description, you should include:

- The final validation loss that was recorded
- A link to an associated learning curve that clearly shows a wallclock-time x-axis that is less than 1.5 hours.
You may either upload an image directly to the repo (use the [./images](./images)) folder or link to a publicly-viewable plot from a service like Weights and Biases.
- A description of what you did

We are considering adding an automated validation loss check, considering it's easy to measure your metrics wrong in a way that will place you higher on the leaderboard than you should be.
If your loss seems too good to be true, make sure to validate your training and valdation datasets are correct, by checking decoded samples, and making sure your vocab is correct with 32k tokens.
It should not be easy to get a validation loss better than 3.3.
We validate at context length 512, so your reported validation loss should also be calculated with this setting.

## OpenWebText (subsample) validation loss leaderboard

<details markdown="1">
<summary>Stanford class leaderboard (Spring 2025)</summary>

| Name           | Validation Loss | Link | Verification status (leave empty) |
| :------------- | --------------: | ---: | --------------------------------: |
| Herman Brunborg | 3.0781| https://api.wandb.ai/links/brunborg-cs336/igorg097 | Verified |
| Stephen Ge | 3.1460 | https://api.wandb.ai/links/stephenge/cc9sewxe | Verified |
| Brandon Snider | 3.1658 | https://api.wandb.ai/links/brandon-snider-stanford-university/v8n2t4py | Verified |
| Joe Li | 3.19406 | [Validation loss curve](images/joe_better_muon.png)
| Tejas Narayanan | 3.22 | https://api.wandb.ai/links/tejas-narayanan/n8itavzy | |
| Hermann Kumbong | 3.22 | https://api.wandb.ai/links/hermannk/iwrvwesk | |
| Ayush Agrawal | 3.261 | https://api.wandb.ai/links/ayushag2410/mcbnccjr | |
| Puheng Li | 3.268 | https://api.wandb.ai/links/puhengli-stanford-university/s1cokosj | |
| Hongyue Li | 3.27| [Validation loss curve](images/hongyue_li.png) | |
| Christine Ye | 3.283 | https://api.wandb.ai/links/christineye/dhqwbfqa | |
| I-han Lai| 3.29|https://wandb.ai/ihan-lai0924-stanford-university/cs336_hw1/reports/owt-validation-loss-25-04-18-01-16-13---VmlldzoxMjM1MjYwNA||
| Prateek | 3.29 | https://wandb.ai/stanfordcs/OWT%20Experiments/reports/--VmlldzoxMjM2NjQ2MQ | |
| Pinlin [Calvin] Xu | 3.29688 | https://api.wandb.ai/links/pinlinxu-lab/rv9m2oqq | |
| Varun Desai | 3.298 | https://wandb.ai/vdesai10/owt_leaderboard/reports/Final-Leaderboard-Submission-Varun--VmlldzoxMjM2NjQ3NA?accessToken=ylvoskxok1cnhegx1i4gziphtc5eih16ylza2buzy13y1uoll58h7jhndr4dviq5 | |
| Michael Bereket | 3.30 | https://api.wandb.ai/links/mbereket/srr1jc5b | |
| Jack Hsieh | 3.3001 | https://wandb.ai/jackellishsieh-stanford-university/cs336-assignment1/runs/ohdb5e0v/panel/mc4jbfhrm?nw=nwuserjackellishsieh | |
| Suze van Adrichem | 3.3134 | https://api.wandb.ai/links/suzevana/nfzefh73 | |
| Chenchen Gu | 3.314 | https://api.wandb.ai/links/cygu/2cwahtxu | |
| Ashish Rao | 3.330 | https://api.wandb.ai/links/aprao/v79845cv | |
| Arnuv Tandon | 3.33213 | https://wandb.ai/arnuv-tandon-stanford-university/cs336/reports/CS-336-Leaderboard--VmlldzoxMjM2NDY5OA?accessToken=eh8nugwo4d6zvq7sgajuni8892vfoomcp7k0klbqzkqrzj6h9ex789r38u76myrh | |
| Mehmet Hamza Erol | 3.353 | https://api.wandb.ai/links/mhamzaerol-stanford-university/hcjj4l7r | |
| Divija Hasteer | 3.35628 | [Validation Loss Curve](images/dhasteer_leaderboard_sub.png) | |
| Christopher Chou | 3.41 | https://api.wandb.ai/links/babychousr-stanford-university/ed9fu89s  | |
| Milan Rohatgi | 3.41 | [[https://api.wandb.ai/links/milanrohatgi/zuet4nhc](https://api.wandb.ai/links/milanrohatgi/abxkie8w)](https://api.wandb.ai/links/milanrohatgi/lq28xt0w) | |
| Katherine Li | 3.418 | https://api.wandb.ai/links/kathli/rmglb4ts |
| Harshvardhan Agarwal |      3.42 | https://api.wandb.ai/links/tokenization/dvezrvbp |  |
| Ramgopal Venkateswaran | 3.44    | https://api.wandb.ai/links/ramvenkat98/cvrfl2pa  |  |
| Ken Liu | 3.47 | https://api.wandb.ai/links/kenziyuliu/3z1f54qp |  |
| Kaitlyn Wang | 3.50 | https://api.wandb.ai/links/kaitwang-stanford-university/wgigpj6h |  |
| Sai Konkimalla | 3.51 | https://api.wandb.ai/links/sai-konk/yf8ashf0 |  |
| Radostin Cholakov | 3.55 | https://api.wandb.ai/links/radi-cho/mrr13237 |  |
| Sally Zhu | 3.55 | https://api.wandb.ai/links/sallyzhu-stanford-university/s6sd95zh |
| Ziqing Huang | 3.55 | https://api.wandb.ai/links/tyltto/505dcz72 | |
| Ayush Alag | 3.56 | https://api.wandb.ai/links/ayushalag1-stanford-university/z56avu3c | |
| Kyler Wang | 3.57 | https://api.wandb.ai/links/kylerwang-stanford-university/5znjvf3e | |
| Adam Zhao | 3.58 | https://api.wandb.ai/links/zhao1adam-stanford-university/5zgjjs1h |
| Aryaman Arora | 3.61 | https://wandb.ai/aryamanarora/cs336/runs/39skvnwk?nw=t6wb3iafj2q |
| Josiah Wong | 3.61 | [Validation loss curve](https://wandb.ai/cremebrule/cs336_leaderboard/reports/CS336-Assignment-1-Initial-Leaderboard-Submission--VmlldzoxMjMxMjU1MA) | |
| orrzohar       |            3.61 |https://api.wandb.ai/links/marvl/xpyqen6p|
| Prateek Varshney | 3.62 | https://api.wandb.ai/links/stanfordcs/jlkmfbgj |
| Varun Desai | 3.63 | https://api.wandb.ai/links/vdesai10/all5y62k | |
| Karthik Dharmarajan | 3.67 | https://wandb.ai/kdharmarajan/cs336-asst1/reports/Validation-Loss-25-04-18-20-41-23---VmlldzoxMjM2NDk1OQ | |
| Shiny Weng |      3.67 | https://api.wandb.ai/links/shinyweng-stanford-university/xt471xol |  |
| Harshit Joshi | 3.69 | https://wandb.ai/josharshit-stanford-university/cs336-basics/reports/CS-336--VmlldzoxMjM2NDcxMQ?accessToken=26yom3e3gznkpvg2yjispit1vhf4thw15i3xbj4hfckynojj0vc2g96bo7uedqec | |
| Harry Shin | 3.70 | https://api.wandb.ai/links/dh2shin2-stanford-university/jueu6en8 | |
| Angikar Ghosal | 3.71 | [Validation loss curve](./images/angikar_owt_bestvalidationloss.png) | |
| Justin Wu   | 3.71 | https://api.wandb.ai/links/justin-wu/9jrz2aep | |
| Harry Shin | 3.70 | https://api.wandb.ai/links/dh2shin2-stanford-university/jueu6en8 | |
| Harshit Joshi | 3.69 | https://wandb.ai/josharshit-stanford-university/cs336-basics/reports/CS-336--VmlldzoxMjM2NDcxMQ?accessToken=26yom3e3gznkpvg2yjispit1vhf4thw15i3xbj4hfckynojj0vc2g96bo7uedqec | |
| Angela Liu | 3.75 | https://api.wandb.ai/links/aliu917/fdx2pwqa  |  |
| Herumb Shandilya | 3.76 | https://wandb.ai/krypticmouse/cs336-basics/runs/1zl172ay?nw=nwuserkrypticmouse | |
| Hongyue Li | 3.79 | [Validation loss curve](./images/lhy.png)  |  |
| atj10 |  3.83 | [Validation loss curve](./images/atj10_loss_curves.png)  |  |
| Ryan Zhao | 3.84 | https://api.wandb.ai/links/knightasterial-stanforduniversity/j7z9j001 | |
| William Huang | 3.88 | https://api.wandb.ai/links/abcisosm/bgl39okf | |
| jshenoy | 3.99 | https://api.wandb.ai/links/jayshenoy-stanford-university/shpznb3o | |
| Arya Bakhtiar | 4.00 | https://drive.google.com/file/d/1nKmlqy1UJ6ZlmWjhZe-jTTN6h4Vn2vZK/view?usp=drive_link | |
| naive baseline |            5.00 |      |                          Verified |

</details>

<details markdown="1">
<summary>Global leaderboard (2025)</summary>

| Name           | Validation Loss | Link | Verification status (leave empty) |
| :------------- | --------------: | ---: | --------------------------------: |
| Jorge Vanco | 2.9393 | https://api.wandb.ai/links/jorgev/qa9to62v | |
| Herman Brunborg | 3.0781| https://api.wandb.ai/links/brunborg-cs336/igorg097 | Verified |
| Vegard Skogstad | 3.1354 | https://api.wandb.ai/links/skogstadv-hobbyist/kvi98ktt | |
| Stephen Ge | 3.1460 | https://api.wandb.ai/links/stephenge/cc9sewxe | Verified |
| Brandon Snider | 3.1658 | https://api.wandb.ai/links/brandon-snider-stanford-university/v8n2t4py | Verified |
| Joe Li | 3.19406 | [Validation loss curve](images/joe_better_muon.png)
| George Grigorev | 3.211 | https://api.wandb.ai/links/thepowerfuldeez/4cxlverq | |
| Tejas Narayanan | 3.22 | https://api.wandb.ai/links/tejas-narayanan/n8itavzy | |
| Hermann Kumbong | 3.22 | https://api.wandb.ai/links/hermannk/iwrvwesk | |
| Ayush Agrawal | 3.261 | https://api.wandb.ai/links/ayushag2410/mcbnccjr | |
| Puheng Li | 3.268 | https://api.wandb.ai/links/puhengli-stanford-university/s1cokosj | |
| Hongyue Li | 3.27| [Validation loss curve](images/hongyue_li.png) | |
| Christine Ye | 3.283 | https://api.wandb.ai/links/christineye/dhqwbfqa | |
| Jiali Yang | 3.28434 | https://api.wandb.ai/links/1021601788-east-china-normal-university/bkrjzfys | |
| I-han Lai| 3.29|https://wandb.ai/ihan-lai0924-stanford-university/cs336_hw1/reports/owt-validation-loss-25-04-18-01-16-13---VmlldzoxMjM1MjYwNA||
| Prateek | 3.29 | https://wandb.ai/stanfordcs/OWT%20Experiments/reports/--VmlldzoxMjM2NjQ2MQ | |
| Pinlin [Calvin] Xu | 3.29688 | https://api.wandb.ai/links/pinlinxu-lab/rv9m2oqq | |
| Varun Desai | 3.298 | https://wandb.ai/vdesai10/owt_leaderboard/reports/Final-Leaderboard-Submission-Varun--VmlldzoxMjM2NjQ3NA?accessToken=ylvoskxok1cnhegx1i4gziphtc5eih16ylza2buzy13y1uoll58h7jhndr4dviq5 | |
| Michael Bereket | 3.30 | https://api.wandb.ai/links/mbereket/srr1jc5b | |
| Jack Hsieh | 3.3001 | https://wandb.ai/jackellishsieh-stanford-university/cs336-assignment1/runs/ohdb5e0v/panel/mc4jbfhrm?nw=nwuserjackellishsieh | |
| Suze van Adrichem | 3.3134 | https://api.wandb.ai/links/suzevana/nfzefh73 | |
| Chenchen Gu | 3.314 | https://api.wandb.ai/links/cygu/2cwahtxu | |
| Ashish Rao | 3.330 | https://api.wandb.ai/links/aprao/v79845cv | |
| Arnuv Tandon | 3.33213 | https://wandb.ai/arnuv-tandon-stanford-university/cs336/reports/CS-336-Leaderboard--VmlldzoxMjM2NDY5OA?accessToken=eh8nugwo4d6zvq7sgajuni8892vfoomcp7k0klbqzkqrzj6h9ex789r38u76myrh | |
| Frank Latos | 3.3506 | https://api.wandb.ai/links/flatos-duo-systems-inc-/c7e7ea70 | |
| Mehmet Hamza Erol | 3.353 | https://api.wandb.ai/links/mhamzaerol-stanford-university/hcjj4l7r | |
| Divija Hasteer | 3.35628 | [Validation Loss Curve](images/dhasteer_leaderboard_sub.png) | |
| Christopher Chou | 3.41 | https://api.wandb.ai/links/babychousr-stanford-university/ed9fu89s  | |
| Milan Rohatgi | 3.41 | [[https://api.wandb.ai/links/milanrohatgi/zuet4nhc](https://api.wandb.ai/links/milanrohatgi/abxkie8w)](https://api.wandb.ai/links/milanrohatgi/lq28xt0w) | |
| Katherine Li | 3.418 | https://api.wandb.ai/links/kathli/rmglb4ts |
| Harshvardhan Agarwal |      3.42 | https://api.wandb.ai/links/tokenization/dvezrvbp |  |
| Ramgopal Venkateswaran | 3.44    | https://api.wandb.ai/links/ramvenkat98/cvrfl2pa  |  |
| Ken Liu | 3.47 | https://api.wandb.ai/links/kenziyuliu/3z1f54qp |  |
| Kaitlyn Wang | 3.50 | https://api.wandb.ai/links/kaitwang-stanford-university/wgigpj6h |  |
| Sai Konkimalla | 3.51 | https://api.wandb.ai/links/sai-konk/yf8ashf0 |  |
| Radostin Cholakov | 3.55 | https://api.wandb.ai/links/radi-cho/mrr13237 |  |
| Sally Zhu | 3.55 | https://api.wandb.ai/links/sallyzhu-stanford-university/s6sd95zh |
| Ziqing Huang | 3.55 | https://api.wandb.ai/links/tyltto/505dcz72 | |
| Ayush Alag | 3.56 | https://api.wandb.ai/links/ayushalag1-stanford-university/z56avu3c | |
| Kyler Wang | 3.57 | https://api.wandb.ai/links/kylerwang-stanford-university/5znjvf3e | |
| Adam Zhao | 3.58 | https://api.wandb.ai/links/zhao1adam-stanford-university/5zgjjs1h |
| Aryaman Arora | 3.61 | https://wandb.ai/aryamanarora/cs336/runs/39skvnwk?nw=t6wb3iafj2q |
| Josiah Wong | 3.61 | [Validation loss curve](https://wandb.ai/cremebrule/cs336_leaderboard/reports/CS336-Assignment-1-Initial-Leaderboard-Submission--VmlldzoxMjMxMjU1MA) | |
| orrzohar       |            3.61 |https://api.wandb.ai/links/marvl/xpyqen6p|
| Prateek Varshney | 3.62 | https://api.wandb.ai/links/stanfordcs/jlkmfbgj |
| Varun Desai | 3.63 | https://api.wandb.ai/links/vdesai10/all5y62k | |
| Karthik Dharmarajan | 3.67 | https://wandb.ai/kdharmarajan/cs336-asst1/reports/Validation-Loss-25-04-18-20-41-23---VmlldzoxMjM2NDk1OQ | |
| Shiny Weng |      3.67 | https://api.wandb.ai/links/shinyweng-stanford-university/xt471xol |  |
| Carl Gieringer | 3.69 | https://api.wandb.ai/links/carl-gieringer-self/9lrupho1 | |
| Harshit Joshi | 3.69 | https://wandb.ai/josharshit-stanford-university/cs336-basics/reports/CS-336--VmlldzoxMjM2NDcxMQ?accessToken=26yom3e3gznkpvg2yjispit1vhf4thw15i3xbj4hfckynojj0vc2g96bo7uedqec | |
| Harry Shin | 3.70 | https://api.wandb.ai/links/dh2shin2-stanford-university/jueu6en8 | |
| Angikar Ghosal | 3.71 | [Validation loss curve](./images/angikar_owt_bestvalidationloss.png) | |
| Justin Wu   | 3.71 | https://api.wandb.ai/links/justin-wu/9jrz2aep | |
| Harry Shin | 3.70 | https://api.wandb.ai/links/dh2shin2-stanford-university/jueu6en8 | |
| Harshit Joshi | 3.69 | https://wandb.ai/josharshit-stanford-university/cs336-basics/reports/CS-336--VmlldzoxMjM2NDcxMQ?accessToken=26yom3e3gznkpvg2yjispit1vhf4thw15i3xbj4hfckynojj0vc2g96bo7uedqec | |
| Angela Liu | 3.75 | https://api.wandb.ai/links/aliu917/fdx2pwqa  |  |
| Herumb Shandilya | 3.76 | https://wandb.ai/krypticmouse/cs336-basics/runs/1zl172ay?nw=nwuserkrypticmouse | |
| Hongyue Li | 3.79 | [Validation loss curve](./images/lhy.png)  |  |
| atj10 |  3.83 | [Validation loss curve](./images/atj10_loss_curves.png)  |  |
| Ryan Zhao | 3.84 | https://api.wandb.ai/links/knightasterial-stanforduniversity/j7z9j001 | |
| William Huang | 3.88 | https://api.wandb.ai/links/abcisosm/bgl39okf | |
| jshenoy | 3.99 | https://api.wandb.ai/links/jayshenoy-stanford-university/shpznb3o | |
| Arya Bakhtiar | 4.00 | https://drive.google.com/file/d/1nKmlqy1UJ6ZlmWjhZe-jTTN6h4Vn2vZK/view?usp=drive_link | |
| naive baseline |            5.00 |      |                          Verified |

</details>
