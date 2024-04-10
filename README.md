# Intoxication Detection using Accelerometer Data

# Project Overview

This project utilizes accelerometer data to distinguish between intoxicated and sober individuals based on their movement patterns. The primary focus is on visualizing permutation entropy and complexity across different segments defined by changes in Transdermal Alcohol Concentration (TAC) readings. The project aims to provide valuable insights into the relationship between alcohol intoxication and physical movements, with potential implications for public health and safety.

## Functions Used

1. `p_entropy(op)`: Computes the permutation entropy of a given ordinal pattern.
2. `s_entropy(freq_list)`: Computes the Shannon entropy of a frequency distribution.
3. `ordinal_patterns(ts, embdim, embdelay)`: Computes ordinal patterns of a time series.
4. `_hash(x)`: Computes a hash value for an array.
5. `complexity(op)`: Computes the complexity of a time series.
6. `calculate_entropy_and_complexity(df_segment, axis)`: Calculates permutation entropy and complexity for a DataFrame segment along a specified axis.
7. `plot_x_y_z(df, title_prefix)`: Plots 'x', 'y', 'z', and 'TAC_Reading' data against time.
8. `plot_entropy_and_complexity(df, title_prefix)`: Plots permutation entropy and complexity for accelerometer data across different segments.

**Formulas Used:**

1) Shannon Entropy (`s_entropy` function): 

![image](https://github.com/priyanka-senthil/Detect_heavy_drinking/assets/160204163/e14a3e76-6986-46b8-bc80-bb8a1475cc27)

    H(X) = Shannon entropy
    pi = Probability of the ith outcome
    n = Total number of possible outcomes

2) Permutation Entropy (`p_entropy` function):

![image](https://github.com/priyanka-senthil/Detect_heavy_drinking/assets/160204163/18326421-09ea-4a5b-baac-34265a2328cd)


    PE: Permutation entropy
    SE: Shannon entropy of ordinal pattern frequency distribution
    N: Number of ordinal patterns


3) Complexity (`complexity` function):

![image](https://github.com/priyanka-senthil/Detect_heavy_drinking/assets/160204163/7268b26a-6230-432e-a55d-e8bc6abb2b02)

    CompJS = Complexity
    Qo = Normalization constant
    JSdivergence = Jensen-Shannon divergence
    pe = Permutation entropy

## Conclusion

This project has demonstrated the efficacy of utilizing accelerometer data to differentiate between intoxicated and sober individuals based on their movement patterns. By visualizing permutation entropy and complexity across segments defined by changes in TAC readings, valuable insights into the relationship between alcohol intoxication and physical movements have been obtained. Moving forward, the integration of machine learning techniques for classification or regression holds promise for enhancing the predictive capabilities of intoxication detection systems, thereby contributing to efforts aimed at mitigating alcohol-related risks and promoting public well-being.

## License

This project is provided under the MIT License. See the `LICENSE` file for details.

