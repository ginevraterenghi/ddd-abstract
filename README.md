GENERAL GUIDELINES FOR MULTIMODAL MARKDOWN TEXTS

PURPOSE
These reusable guidelines describe how to write texts that combine prose, formatting, references, and multimedia within a web-based reading experience. Adapt the structure and media choices to each new text. Do not assume that a renderer supports a syntax without testing it.

1. TEXT STRUCTURE
Write coherent prose in the order in which readers should encounter it. When a continuous-text layout is required, use one uninterrupted paragraph without blank lines or separate headings. For other projects, paragraph breaks are allowed: insert one empty line between paragraphs. Integrate media at the point where it contributes to the meaning, preserving readable punctuation and spacing.

2. BASIC MARKDOWN FORMATTING
Normal text: Text
Italic: *Text*
Bold: **Text**
Bold italic: ***Text***
Use emphasis selectively to support hierarchy and interpretation.

3. COLOURED TEXT (CUSTOM SYNTAX)
{crimson|Text}
{green|Text}
These colour directives are specific to the documented renderer, not standard Markdown. Apply them consistently and check that nested formatting works in the target site.

4. EXTERNAL LINKS
[Visible link text](https://example.com)
Use meaningful link labels.

5. MULTIMODAL ANNOTATIONS (DOCUMENTED CUSTOM SYNTAX)
General: [[visible text|content]]
With optional emoji: [[visible text|content|emoji]]
Image annotation: [[View image|image.jpg|📷]]
Video annotation: [[Watch video|video.mp4|🎬]]
Audio annotation: [[Listen|audio.mp3|🔊]]
External resource: [[Explore resource|https://example.com]]
Text annotation: [[Read more|Additional contextual information.|✶]]
The visible text acts as the annotation label. Use this form when an interactive reference is intended; do not confuse it with an image embedded directly in the text.

6. DIRECTLY EMBEDDED MEDIA (REQUIRES RENDERER SUPPORT)
Standard Markdown image: ![Descriptive alternative text](image.jpg)
HTML video: <video src="video.mp4" controls></video>
HTML audio: <audio src="audio.mp3" controls></audio>
These are candidate embedding syntaxes, not confirmed features of the supplied custom renderer. Inline thumbnail sizing, hover enlargement, overlays that retain the text background, and compact media players are presentation behaviours controlled by the website's HTML/CSS/JavaScript. They cannot be guaranteed by Markdown alone. Test each media type in the target site before publication.

7. BIBLIOGRAPHIC REFERENCES
Keep references consistent and close to the claims they support. If the target template displays references directly, a possible visible convention is (■ Author, Year). If bibliographic references should open additional information, use the documented annotation pattern, for example [[■ Author, Year|Full reference details|✶]]. The exact bibliography rendering is template-dependent; do not invent full citations or assume either display mode is automatically supported.

8. SECTION LABELS AND PROMPTS WITHIN PROSE
For a continuous text, a short bold label can introduce a theme: **Theme name**. A question can be italicised: *What does this reveal?* If supported and appropriate, combine a coloured span and a symbol: {crimson|*✶ What does this reveal?*}. Symbols and colours are editorial choices, not mandatory formatting rules.

9. MEDIA FILES AND PATHS
Use descriptive, stable filenames and correct relative paths. Common formats include JPG/PNG/WebP for images, MP4 for video, and MP3 for audio, subject to browser and site support. Ensure that assets exist at the specified paths. Include alternative text for meaningful images, and provide captions or transcripts when needed for accessibility.

10. EDITORIAL AND TECHNICAL CHECKS
Preserve the intended wording, punctuation, and media order. Avoid making ordinary words clickable unless they are meant to be links or annotation triggers. Confirm that every image, audio file, video, and citation renders correctly. Test on desktop and mobile, including keyboard and touch interaction. Verify that any enlargement or overlay behaves as intended without hiding essential context.

SOURCE STATUS
The uploaded README documents Markdown emphasis, the custom colour syntax, external links, paragraph breaks, and [[...]] multimedia annotations. Direct inline images, HTML video/audio elements, hover-to-enlarge effects, and the exact visual treatment of bibliographic references are not established by that README and require confirmation against the site's implementation.