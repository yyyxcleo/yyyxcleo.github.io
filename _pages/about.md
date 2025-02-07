
Brief Introduction
======
☺️I am a third-year undergraduate student majoring in Software Engineering at Harbin Institute of Technology. My research interests include continual learning, video and image processing, image generation, and multimodal learning. At my university, I have participated in research at the ICES Lab under the guidance of [Prof. Chunshan Li](https://homepage.hit.edu.cn/lichunshan?lang=zh). Additionally, I have interned at Westlake University advised by [Prof. Ziqing Li](https://www.westlake.edu.cn/faculty/stan-zq-li.html), and at the OV³Lab at Peking University advised by [Prof. Jiahuan Zhou](https://www.icst.pku.edu.cn/xztd/xztd_01/1354287.htm).


## Research Experience

### 🌈Deep Priors Driven Posterior Sampling in Diffusion Models  
**Duration:** 2024.03--2024.06  
**Role:** Core Member  
- Proposed a deep prior-driven method to address the linear inverse problem in diffusion models.
- Improved image restoration capability by guiding the diffusion process with deep neural networks.
- Conducted denoising, inpainting, and colorization experiments on the FFHQ face dataset, using PSNR and LPIPS as evaluation metrics, and achieved better performance compared to previous works.

### 📹National College Student Innovation Training Project — Remote Sensing Meteorological Video Prediction  
**Duration:** 2024.03--2024.06  
**Role:** Core Member  
- Utilized spatiotemporal sequence prediction models to address the problem of accurately predicting cloud changes and weather conditions.
- Extracted spatiotemporal features from cloud video data to learn dynamic movement patterns of cloud layers.

### 🧪Prototype-based Dual-Dimensional Knowledge Distillation for Online Continual Learning  
**Duration:** 2024.11--2025.02  
**Role:** First Author  
- Proposed an optimization method combining prototype-based dual-dimensional knowledge distillation to balance model learning ability and forgetting resistance in online continual learning.
- Conducted classification experiments on standard datasets like CIFAR-100, demonstrating superior performance in terms of average accuracy and forgetting rate compared to existing baseline models.
- The paper is currently under review for a CCF-C conference.


Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
