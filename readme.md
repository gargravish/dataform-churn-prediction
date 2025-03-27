# Churn Prediction for Mobile Application

## Execution

To execute the Dataform project and run the churn prediction pipeline:

1.  **Run all actions:** Use the command `dataform run` to execute all Dataform actions, including data processing, model training, and prediction.
2.  **Monitor execution:** Monitor the execution in the Dataform web UI or CLI output to ensure all steps complete successfully.

## Results and Evaluation

After successful execution, the churn predictions for the test dataset will be available in the `user_propensity.best_model_predict` view in your BigQuery project.

To evaluate the model's performance:

1.  **Access predictions:** Query the `user_propensity.best_model_predict` view to retrieve the predicted churn probabilities for each user in the test set.
2.  **Compare with actual churn:** Compare the predictions with the actual churn labels (available in the `df_train_eval_test_data` view for the "TEST" split) to assess the model's accuracy.
3.  **Calculate evaluation metrics:** Calculate relevant evaluation metrics such as precision, recall, F1-score, and AUC to quantify the model's performance.

## Future Improvements

*   **Feature engineering:** Explore additional features or transformations of existing features to potentially improve model accuracy.
*   **Hyperparameter tuning:** Conduct more extensive hyperparameter tuning for the machine learning models to optimize their performance.
*   **Model comparison:** Evaluate and compare other machine learning algorithms beyond those currently implemented.
*   **Real-time prediction:** Investigate methods for generating real-time churn predictions for new users as they interact with the application.
*   **A/B testing:** Design and conduct A/B tests to measure the impact of interventions based on churn predictions.
