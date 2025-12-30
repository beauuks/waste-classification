# Trash Classification

This project builds a **two-stage waste classification system** to sort trash images more accurately and efficiently.

## Project Overview

The pipeline works in **two steps**:

1. **Binary Classification (Organic vs Recyclable)**  
   The first model predicts whether the trash is **organic** or **recyclable**.  
   This helps route the item to the correct next step (organic waste can be handled immediately, while recyclable waste needs more detailed sorting).
   - CNN

3. **Multiclass Classification (Recyclable Sub-categories)**  
   If the item is predicted as **recyclable**, a second model further classifies it into specific recyclable categories (cardboard, plastic, paper, metal, glass).
   - CNN
   - MobileNetV2

Finally, both models are combined into a single end-to-end workflow so you can input an image and get the final waste label.


## Key Features
Two-stage classification for practical waste sorting
- First stage separates **organic vs recyclable**
- Second stage refines **recyclable** items into detailed categories
- Modular design (easy to improve models or add new classes)


## Tech Stack
- Python
- Jupyter Notebook
- ML/DL libraries (NumPy, Pandas, Scikit-learn, TensorFlow)


## How It Works

1. Input an image
2. Model 1 predicts: **Organic** or **Recyclable**
3. If **Organic** → output result
4. If **Recyclable** → Model 2 predicts the recyclable category → output final result


## Future Improvements
- Expand recyclable categories with more data
- Multi-object detection


## License

This project is intended for educational and research purposes.
