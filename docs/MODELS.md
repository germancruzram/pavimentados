# Pavimentados system models
---

## Detection of pavement failures
---

This model is based on Yolo version 8, which allows to identify objects or elements within an image. 
It was retrained from a base model to detect 8 types of faults:

1. Longitudinal Linear Cracks (D00): these are cracks in the pavement that are longitudinally located.
2. Transverse Linear Cracks (D10): These are cracks in the pavement that are transversely located.
3. Crocodile skin: These are clusters (D20) of fissures that are usually found in blocks in such a way that they look like the scaly skin of a crocodile.
4. Protrusions or Potholes (D40): These are holes found in the pavement that may or may not be scaled.
5. Cross walk blur (D44): Occurs when the delineation or demarcation on the pavement is out of focus or blurred.
6. White line blur (D43): Occurs when the delineation or demarcation on the pavement is out of focus or blurred.

The model returns the following information:
 - Class of the identified object
 - Location within the image
 - Probability with which that detection is considered

> **Note**: This model was retrained using the folowing base model: [RoadDamageDetection](https://github.com/oracl4/RoadDamageDetection).

## Detection of signals
---

This model is based on Yolo version 11, which allows to identify objects or elements within an image. 
It was retrained from a base model to detect 10 types of signals:

1. PREVENCION
2. REGLAMENTARIA
3. INFORMATIVA
4. CURVA
5. PERMITE
6. OBRA
7. PROHIBICION
8. ADVERTENCIA
9. STOP
10. CEDAPASO

The model returns the following information:
 - Class of the identified object
 - Location within the image
 - Probability with which that detection is considered
