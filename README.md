# ShopLook
**ShopLook**, a computer vision-based system that helps online shoppers find fashion items similar to those worn by models in e-commerce product images. Instead of just recommending alternatives for a single item (e.g., a T-shirt), it suggests **the entire outfit**, including shoes, shorts, or jackets.


### **Why is This Important?**
- Many people see a model wearing an outfit online and want to buy everything in that look.
- Current recommendation systems usually suggest similar products only for the main item, not the full outfit.
- **ShopLook** improves the shopping experience by allowing users to "shop the look" and helps boost cross-selling.

---

### **How Does It Work?**  
The system follows **four key steps**:

1. **Human Keypoint Detection** 👤  
   - It detects key body points (head, ankles, etc.) to identify **full-body images** of models wearing outfits.

2. **Pose Classification** 📷  
   - It ensures the model is facing forward for a clear view of all clothing items.

3. **Fashion Article Detection & Localization** 👕👟  
   - The system detects individual clothing items (e.g., shirts, jeans, shoes) in the image using an AI model called **Mask R-CNN**.
   - **Active learning** helps improve accuracy by retraining on incorrectly classified items.

4. **Image Similarity & Recommendations** 🔍  
   - A **triplet network model** (a deep learning technique) is used to match the detected clothing items with similar products from Myntra’s catalog.
   - The system ranks recommendations based on similarity.

---

### **Future Improvements**
- Adding occasion-based recommendations (e.g., workwear, partywear).
- Considering finer details like sleeve length, collar type, etc.

---

### **Conclusion**
This project presents an AI-driven solution to improve fashion e-commerce recommendations. By using **computer vision and deep learning**, ShopLook allows users to buy an entire outfit, making online shopping more engaging and profitable.

Reference:
https://arxiv.org/pdf/2008.11638
