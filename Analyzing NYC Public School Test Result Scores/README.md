![schoolbus](https://github.com/Aakaaaassh/SQL/assets/66636545/b926889c-3f2b-47fa-8128-f74238b3412b)
<html>
<body>
<!--StartFragment--><p style="box-sizing: border-box; margin: 1em 0px 0px; text-align: left; color: rgb(0, 0, 0); font-family: &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">Photo by<span> </span><a href="https://unsplash.com/@jannis_lucas" target="_blank" style="box-sizing: border-box; background-color: transparent; color: rgb(51, 122, 183); text-decoration: underline;">Jannis Lucas</a><span> </span>on<span> </span><a href="https://unsplash.com/" target="_blank" style="box-sizing: border-box; background-color: transparent; color: rgb(51, 122, 183); text-decoration: underline;">Unsplash</a>.<br style="box-sizing: border-box;"></p><p style="box-sizing: border-box; margin: 1em 0px 0px; text-align: left; color: rgb(0, 0, 0); font-family: &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">Every year, American high school students take SATs, which are standardized tests intended to measure literacy, numeracy, and writing skills. There are three sections - reading, math, and writing, each with a maximum score of 800 points. These tests are extremely important for students and colleges, as they play a pivotal role in the admissions process.</p><p style="box-sizing: border-box; margin: 1em 0px 0px; text-align: left; color: rgb(0, 0, 0); font-family: &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">Analyzing the performance of schools is important for a variety of stakeholders, including policy and education professionals, researchers, government, and even parents considering which school their children should attend.</p><p style="box-sizing: border-box; margin: 1em 0px 0px; text-align: left; color: rgb(0, 0, 0); font-family: &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">In this notebook, we will take a look at data on SATs across public schools in New York City. Our database contains a single table:</p><h1 id="schools" style="box-sizing: border-box; font-size: 25.998px; margin: 1.08em 0px 0px; font-family: &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-weight: bold; line-height: 1; color: rgb(0, 0, 0); font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;"><code style="box-sizing: border-box; font-family: monospace; font-size: 25.998px; padding: 0px; color: rgb(0, 0, 0); background-color: rgb(255, 255, 255); border-radius: 2px; white-space: pre-wrap; border: 0px;">schools</code><a class="anchor-link" href="https://sessions.datacamp.com/proxy/absolute/3d6365a9-e8b4-47aa-93f6-972a2e8b8c68/notebooks/production/users/4664114/qj232w0ahw/notebooks/notebook.ipynb#schools" style="box-sizing: border-box; background-color: transparent; color: rgb(51, 122, 183); text-decoration: none; padding: 0px 20px; visibility: hidden;"></a></h1>

column | type | description
-- | -- | --
school_name | varchar | Name of school
borough | varchar | Borough that the school is located in
building_code | varchar | Code for the building
average_math | int | Average math score for SATs
average_reading | int | Average reading score for SATs
average_writing | int | Average writing score for SATs
percent_tested | numeric | Percentage of students completing SATs

<p style="box-sizing: border-box; margin: 1em 0px 0px; text-align: left; color: rgb(0, 0, 0); font-family: &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(255, 255, 255); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;">Let's familiarize ourselves with the data by taking a looking at the first few schools!</p><!--EndFragment-->
</body>
</html>
Photo by [Jannis Lucas](https://unsplash.com/@jannis_lucas) on [Unsplash](https://unsplash.com/).

Every year, American high school students take SATs, which are standardized tests intended to measure literacy, numeracy, and writing skills. There are three sections - reading, math, and writing, each with a maximum score of 800 points. These tests are extremely important for students and colleges, as they play a pivotal role in the admissions process.

Analyzing the performance of schools is important for a variety of stakeholders, including policy and education professionals, researchers, government, and even parents considering which school their children should attend.

In this notebook, we will take a look at data on SATs across public schools in New York City. Our database contains a single table:

schools
column	type	description
school_name	varchar	Name of school
borough	varchar	Borough that the school is located in
building_code	varchar	Code for the building
average_math	int	Average math score for SATs
average_reading	int	Average reading score for SATs
average_writing	int	Average writing score for SATs
percent_tested	numeric	Percentage of students completing SATs
Let's familiarize ourselves with the data by taking a looking at the first few schools!