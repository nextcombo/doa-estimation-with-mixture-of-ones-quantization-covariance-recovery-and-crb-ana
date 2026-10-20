# DOA Estimation with Mixture of Ones Quantization: Covariance Recovery and CRB Analysis [with MATLAB Code]

1. Title: Covariance Recovery and CRB Analysis for DOA Estimation by Mixed One-bit Quantized Signals
2. Abstract: Doppler of arrival (DOA) estimation is a fundamental task in array signal processing. Although one-bit quantization significantly reduces hardware complexity and cost, it introduces a large amount of quantization errors, which degrades the estimation accuracy. To alleviate this issue, this paper proposes a hybrid one-bit quantization method that integrates one-bit quantized sensors with full-resolution sensors. It derives the theoretical relationship expression between the mixed one-bit quantized observation values and the pre-quantization covariance matrix, achieving reliable reconstruction to support subsequent DOA estimation. Additionally, a corresponding CRB is constructed to characterize the theoretical performance of the proposed method. Experimental results show that this method consistently outperforms one-bit quantization in DOA estimation tasks and can effectively preserve signal features, enhancing downstream processing capabilities such as target recognition.
3. Introduction: Doppler of arrival (DOA) estimation is a key technology for determining the angle of the signal source relative to the receiving array, widely applied in wireless communication, acoustic positioning, radar, security surveillance, and robotic navigation.
4. Common DOA estimation methods (such as MUSIC algorithm, ESPRIT algorithm) typically require sampling and quantization before digital processing. The higher the quantization resolution, the higher the power consumption and hardware cost, and it generates more data volume, increasing storage and computational complexity.
5. One-bit quantization, as a cost-saving technology, reduces analog frontend costs and complexity by minimizing the bit depth required for representing analog signals, especially suitable for large-scale antenna arrays. However, as an extreme form of quantization, one-bit quantization introduces significant quantization errors, affecting DOA estimation accuracy and performance decline in tasks such as target recognition.
To reduce quantitative errors, methods for low-resolution and hybrid resolution quantization have been proposed. However, the cost savings from hardware reduction are far less than one-bit quantization. Additionally, modifying array structure (such as sparse arrays) can improve performance without significantly increasing costs, but there are still issues with estimation biases associated with these methods.
In practical applications, after DOA estimation, it is often necessary to perform signal processing tasks such as target recognition, tracking, and ranging. Therefore, retaining as many signal features as possible is crucial.
In summary, while one-bit quantization significantly reduces hardware complexity, it faces two major challenges: firstly, quantization errors lead to decreased accuracy in DOA estimation; secondly, it is difficult to preserve the signal features required by downstream tasks. To address this, this paper proposes a hybrid quantization method that integrates one-bit quantization with full-resolution sensors, maintaining low hardware complexity while enhancing signal fidelity. This method is applicable to various linear array structures such as ULA, NLA, and interleaved arrays.
The contributions of this paper include: deriving closed-form recovery formulas to reconstruct the covariance matrix before quantization from the covariance of mixed one-bit quantized observations, supporting subspace-based DOA estimation methods like MUSIC; deriving the CRB of the proposed method, providing a theoretical performance benchmark between one-bit quantization and full-resolution quantization; and verifying through extensive experiments on ULA, NLA, and interleaved arrays that the proposed method consistently outperforms one-bit quantization in DOA estimation accuracy, requiring only a small number of full-resolution sensors to achieve good trade-offs in performance and hardware cost, and allowing individual full-resolution sensors to retain critical information for target recognition tasks.
Method Introduction:
1. Core idea: In sensor arrays, some sensors use full-resolution quantization (index set), while others use one-bit quantization (index set), with both types of sensors not overlapping and covering all sensors. By distinguishing the covariance calculation methods for different quantization types of sensors, the complete covariance matrix before quantization is reconstructed, which is then used for DOA estimation. The CRB of this method is derived as a performance benchmark.
2. Key steps:
• Covariance restoration: Different from other methods, the corresponding restoration formula is used based on the type of sensor quantization.
•  
Full Resolution Sensors: Before and after quantization, the covariance is approximately equal, i.e.;
•  
A Quantization-based Intersensor (QI) method: Based on the law of square root, the real and imaginary parts of the quantized covariance are used to recover the original covariance.
•  
Mixed Quantization Sensor Interaction (or vice versa): Reconstruct the original covariance by multiplying the real and imaginary parts of the post-quantized covariance.
•  
CRB Derivation: For deterministic signals, the snapshot model is decomposed into real and imaginary parts, defining the correlation matrix and projection operator. The CRB for DOA estimation under mixed-bit quantization is derived, with diagonal elements of the quantization matrix set according to the sensor quantization type.
V. Conclusion This paper proposes a hybrid one-bit quantization method for DOA estimation, which is based on the combination of a small number of full-resolution sensors and one-bit quantized sensors, while maintaining low hardware complexity and preserving key signal characteristics.
The closed-form recovery formula and corresponding CRB for the pre-quantized covariance matrix are derived, providing theoretical support for method performance. Extensive experimental validation indicates that this method consistently outperforms one-bit quantization in DOA estimation accuracy across various structures including ULA, NLA, and commutative arrays, with the CRB being between full-resolution quantization and one-bit quantization.
Even with only a few full-resolution sensors, this method can achieve good trade-offs between performance and hardware cost while effectively preserving signal characteristics and enhancing the reliability of downstream tasks such as target recognition.
This hybrid quantization method provides a practical solution for resource-constrained scenarios (such as drone surveillance, edge radar systems, and intelligent sensor networks), balancing power efficiency with signal integrity.
End

## Images

![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](01.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](02.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](03.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](04.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](05.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](06.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](07.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](08.jpg)
![[DOA Estimation] Mixture of Ones Quantization: Covariance Recovery and CRB Analysis for DOA Estimation [with MATLAB Code]](09.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
