## Main claims

NOTE: Models that were trained without positional embeddings will be referred to as "ablated models" and models trained with them will be referred to as "intact models" 

- Spatial structure in attention emerges primarily from consistent patch ordering during training; positional embeddings do not create this structure but systematically sharpen and stabilize it.

- Positional embeddings causally increase the effective dimensionality and heterogeneity of the residual stream during training, which in turn contributes significantly, but not exclusively, to improved robustness under distribution shift.

- Models ablated of their positional embeddings retain spatial structure, indicating that they rely on patch statistics and content-based correlations rather than explicit positional coordinates.

- Distributional shifts such as stylization disrupt the patch-statistics-based spatial strategy used by ablated models; combined with their low residual dimensionality, this leads to uniform token similarity and degraded robustness.

- Positional embeddings appear to thicken class manifolds by supporting higher-dimensional and less entangled representations, reducing class-specific collapse under perturbation.