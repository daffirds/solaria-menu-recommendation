# Solaria Personalized Menu Recommendation System 🍜

This project builds a recommendation system for menu items in *Solaria* restaurants based on customer ratings using Singular Value Decomposition (SVD).

## Project Structure
- `data/` : datasets used in the project.
- `notebooks/` : Jupyter notebooks with exploratory analysis and experiments.
- `plot/` : Saved plots.

## Methods
- SVD-based matrix factorization
- Iterative imputation for missing ratings
- Folding-in method for new users in latent factor models (SVD model)

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/daffirds/solaria-menu-recommendation.git
   cd solaria-menu-recommendation
````

2. Open the Jupyter notebook:

   ```bash
   jupyter notebook notebooks/svd_recommendation.ipynb
   ```
3. Run **all cells** in the notebook to set up the recommendation system.

4. Input your ratings for the 20 menu items by creating a list, for example:

```python
rating = [0, 0, 1, 2, 4, 5, ..., 2]  # replace ... with your ratings until all 20 items
```

5. Run the recommendation function:

```python
show_recom(rating)
```

This will display the recommended menu items based on your ratings.

## Requirements

* Julia 1.11.5
* Packages: `CSV`, `DataFrames`, `LinearAlgebra`, `Plots`, `BenchmarkTools`, `Dates`, `ColorSchemes`, `Random`

## Team

This project is a collaborative effort for **Mathematical Computing Applications Course** at **IPB University**.

* **Team Members (Students):**

  * Cantik Almira M. Z. 
  * Nurani Candra W. 
  * Daffa Firdaus (@daffirds)
  * Vera Tifani E.
  * Dicky Arya A. S.
  * Novita Aprilia P.
  
* **Advisors (Lecturers):**

  * Sri Nurdiati
  * Mohamad Khoirun N.

## Paper

This project is described in more detail in the following paper:  
[https://journal.unesa.ac.id/index.php/jram/article/view/38789](https://journal.unesa.ac.id/index.php/jram/article/view/38789)

## License

This project is licensed under the MIT License.