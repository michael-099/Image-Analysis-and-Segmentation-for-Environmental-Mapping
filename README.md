
# Image Analysis and Segmentation for Environmental Mapping

### Objective

The objective of this lab assignment is to develop an image analysis pipeline using undirected graphical models to map environmental features surrounding a specified location. This includes retrieving satellite imagery, segmenting relevant features such as forests and grassy areas, and visualizing them with color-coded boundaries. Additionally, the assignment includes printing the elevation of the specified location (building).

### Tasks

#### 1. Retrieval of Satellite Imagery:

- Utilize satellite imagery APIs or datasets to retrieve high-resolution images of a specified location.
- Define the center coordinates of the location and specify the radius for image retrieval (1000 ft).

#### 2. Retrieval of Elevation Information:

- Utilize elevation APIs or datasets (e.g., Google Maps Elevation API)to retrieve the elevation of the specified location (building).
- Print the elevation value for further analysis and interpretation.

#### 3. Image Processing and Segmentation:

- Preprocess the retrieved satellite image to ensure consistent resolution and format (350x350 pixels).
- Implement an undirected graphical model to analyze the image and identify relevant environmental features, including forests and grassy areas.
- Define nodes to represent pixels in the image and edges to capture spatial relationships.
- Incorporate potential functions to detect clusters of trees or vegetation, as well as grassy areas, utilizing color, texture, or shape features.
- Implement inference algorithms (e.g., belief propagation) to perform segmentation and identify regions corresponding to trees, grass, or other features.

#### 4. Visualization of Environmental Features:

- Draw an edge from the specified location to the identified cluster of trees using the undirected model.
- Define color-coded boundaries around the detected forest regions based on distance from the location:
  - Draw a blue circle around forests within 200 ft radius.
  - Draw a red circle around forests between 200 ft and 1000 ft radius.
- Similarly, draw color-coded boundaries around detected grassy areas.
- Ensure visual clarity and accuracy in depicting the boundaries of the detected regions.

#### 5. Evaluation and Analysis:

- Evaluate the effectiveness of the image analysis and segmentation pipeline in identifying forested areas, grassy areas, and other features surrounding the specified location.
- Compare the results with ground truth data or reference datasets if available.
- Analyze the impact of different parameters and potential functions on the segmentation performance.
- Discuss potential applications and implications of the developed pipeline for environmental mapping and monitoring.

#### 6. Documentation and Reporting:

- Document the implementation details, including preprocessing steps, model formulation, and visualization techniques.
- Provide code snippets or scripts demonstrating the retrieval, processing, and segmentation of satellite imagery.
- Include visualizations of the detected forest regions, grassy areas, and other features with color-coded boundaries.
- Write a detailed report summarizing the findings, including evaluation results, analysis of segmentation performance, and potential improvements.

---

### Additional Challenges (Optional)

- Extend the pipeline to detect and segment additional environmental features such as water bodies, urban areas, or agricultural fields.
- Explore advanced techniques for feature extraction and representation, such as deep learning-based approaches.
- Integrate the pipeline with geographic information systems (GIS) for interactive visualization and analysis of environmental data.

---

### Submission Guidelines

- Submit the report documenting the implementation and evaluation of the image analysis pipeline.
- Include any relevant source code, scripts, or notebooks used in the development process.
- Optionally, provide supplementary materials such as presentation slides or a demo video showcasing the functionality of the pipeline.

---

### Resources

- Satellite imagery APIs or datasets (e.g., Google Earth Engine, Sentinel Hub).
- Elevation APIs or datasets (e.g., Google Maps Elevation API) for retrieving location elevation data.
- Image processing libraries (e.g., OpenCV, scikit-image) for preprocessing and analysis.
- Graphical model libraries (e.g., NetworkX, PyTorch) for implementing undirected graphical models.
