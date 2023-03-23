# deeplearning-assignment-7
Video Link: https://drive.google.com/drive/folders/10VJ0v-iTyxgjkoWVFWVq7zgRPNEqb6vq?usp=share_link

Description: 
1) 1.	Follow the instruction below and then report how the performance changed.(apply all at once) 
• Convolutional input layer, 32 feature maps with a size of 3×3 and a rectifier activation function. 
• Dropout layer at 20%.
 • Convolutional layer, 32 feature maps with a size of 3×3 and a rectifier activation function. • Max Pool layer with size 2×2. 
• Convolutional layer, 64 feature maps with a size of 3×3 and a rectifier activation function. • Dropout layer at 20%. 
• Convolutional layer, 64 feature maps with a size of 3×3 and a rectifier activation function. • Max Pool layer with size 2×2. 
• Convolutional layer, 128 feature maps with a size of 3×3 and a rectifier activation function. • Dropout layer at 20%. 
• Convolutional layer,128 feature maps with a size of 3×3 and a rectifier activation function. • Max Pool layer with size 2×2. 
• Flatten layer. 
• Dropout layer at 20%. 
• Fully connected layer with 1024 units and a rectifier activation function. 
• Dropout layer at 20%. 
• Fully connected layer with 512 units and a rectifier activation function. 
• Dropout layer at 20%. 
• Fully connected output layer with 10 units and a Softmax activation function Did the performance change?

2. Predict the first 4 images of the test data using the above model. Then, compare with the actual label for those 4 images to check whether or not the model has predicted correctly.
"# Predict the first 4 images of the test data\n",
        "predictions = model.predict(X_test[:4])\n",
        "# Convert the predictions to class labels\n",
        "predicted_labels = numpy.argmax(predictions, axis=1)\n",
        "# Convert the actual labels to class labels\n",
        "actual_labels = numpy.argmax(y_test[:4], axis=1)\n",
        "\n",
        "# Print the predicted and actual labels for the first 4 images\n",
        "print(\"Predicted labels:\", predicted_labels)\n",
        "print(\"Actual labels:   \", actual_labels)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri"
        },
        "id": "vvcyfHmUzJ2n",
        "outputId": "a39a54f1-43d3-4e60-aa47-abeedd908e1b"
      },
      "execution_count": 18,
     
            
            3)Visualize Loss and Accuracy using the history object
          In this we have ploted the Validation loss 
          Accuracy 
          Model loss
          Upper right 
          lower right 
          plt.show (n)
          
