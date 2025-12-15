# Text-to-CAD
Python-based CAD generation tool that converts natural-language text prompts into fully parametric 3D CAD models. the project supports common engineering primitives (cubes, cylinders, plates, spheres, tubes)  assigning sensible default dimensions, and exporting models in STL and STEP formats.

<h1>Description:</h1>

The AI CAD Generator is a Python-based project that leverages CadQuery to produce 3D models from text prompts without relying on cloud APIs. The system uses offline AI techniques for intent detection and parameter parsing, allowing users to generate CAD models of engineering primitives using natural language. The backend is modular, enabling future expansion to complex mechanical parts such as bolts, threads, and assemblies.

A Jupyter Notebook interface provides a user-friendly frontend with a text input box, generate button, and options to download STL and STEP files, making the tool accessible even for beginners.

<h2>Key Features:</h2>

Generate parametric 3D CAD models from natural-language prompts.

Offline AI for shape classification and parameter extraction (no API key required).

Supports cubes, cylinders, spheres, plates, and tubes.

Automatic default dimensions and geometry validation.

Export models to STL and STEP formats.

Modular architecture for easy extension to more complex shapes.

Jupyter Notebook user interface with text input and download buttons.

<h2>Future Improvements:</h2>

<b>Expanded Shape Library:</b> Add support for bolts, threads, cones, and more complex mechanical parts.

<b>Advanced AI Parsing:</b> Improve prompt understanding using offline ML models for more natural prompts.

<b>User Interface Enhancements:</b> Add progress indicators, interactive sliders, and visual previews.

<b>Web Deployment:</b> Convert to Streamlit or Gradio web app for easier online usage.

<b>Performance Optimization:</b> Ensure fast generation for large or complex models.

<h2>Challenges:</h2>

Designing an intuitive frontend for non-technical users.

Handling ambiguous or incomplete prompts with sensible defaults.

Ensuring offline AI parsing is accurate for a wide variety of user inputs.

<h2>Walkthrough</h2> <p align="center">

The notebook interface before generating a model:<br/>

<img src="https://imgur.com/0CL3uER.png" height="60%" width="70%" alt="AI CAD Generator UI"/>

<br/><br/>

User enters a text prompt, e.g., 'tube outer 30 inner 26 height 60', then clicks generate:<br/>

<img src="https://imgur.com/X4cxc6K.png" height="80%" width="80%" alt="Text-to-CAD Prompt"/>

After generating, user can download STL or STEP files.

<br/><br/>

User could also enter a prompt e.g., 'A cylinder with height 20mm.' The module suggest default dimensions for the diameter:<br/>

<img src="https://imgur.com/z4SMn78.png" height="80%" width="80%" alt="Cylinder, default diameter"/>

<br/><br/>

<b>Note:</b> The project is fully offline, and users can safely experiment with their own prompts and parameters to generate CAD models.
