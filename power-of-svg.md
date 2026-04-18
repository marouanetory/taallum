
# Generating free body diagram with AI

## Problem:
When we try to generate pictures with LLM, it is often inaccurate, deformed, riddled with wrong shapes due to the nature of how computationally expensive to draw pixel and the lack of accurate methods to verify it. LLM is blind, it cannot see unless the result is out and you upload it again to verify it. It will still struggle over and over to make it.
## Solution:
AI is getting better and better at Math. We can leverage this capability by using SVG* format. SVG is made of geometrical shape therefore as long as AI can think through it the right way, it can spot errors in a systematic manner and redraw it in the proper positions just by adjusting numbers. It can happens in just one inference.
> “Scalable Vector Graphics (SVG) is an XML-based vector graphics format for defining two-dimensional graphics, having support for interactivity and animation.” – Wikipedia https://en.wikipedia.org/wiki/SVG
## Method:
We can demonstrate the following capability with these examples. <br/>
**Prompt:** make a high density SVG code of an inclined plane in physics. this is a complex problem.

Model: Gemini 3.1 pro <br/>
<img width="640 " height="1280" alt="gemini 3.1 pro svg inclined plane physics" src="https://github.com/user-attachments/assets/a163c471-93c9-43a9-85c4-0000d0c394f6" />

This method was tested but it did not work on Gemini 3.1 flash, Chatgpt GPT5.4-instant GPT5.4-thinking Kimi k2.5 instant, and Kimi k2.5 thinking. 

## Failed attempts:
**Prompt:** make a high density SVG code of an inclined plane in physics. this is a complex problem. <br/>

Model: Kimi k2.5 thinking<br/>
<img width="640 " height="1280" alt="kimi k2.5 thinking svg inclined plane physics" src="https://github.com/user-attachments/assets/d1dffb30-8ec8-4e66-a30a-e41a45b91562" />
<br/>
*Prompt:* make a high density SVG code of an inclined plane in physics. this is a complex problem. <br/>

Model: Gemini 3 flash  <br/>
<img width="640 " height="1280" alt="Gemini 3 flash svg inclined plane physics" src="https://github.com/user-attachments/assets/944d48f0-5bae-46fa-8e3e-978c0d26bbd8" />

