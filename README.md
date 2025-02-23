## Inventory Optimization using Simulation Approach

The "Inventory Optimization with DES Simulation and Genetic Algorithms" repository is a comprehensive tool designed for inventory scientists and developers aiming to enhance inventory management through advanced simulation and optimization techniques. By integrating Discrete Event Simulation (DES) with Genetic Algorithms (GA), this project offers a robust framework to model, analyze, and optimize inventory systems, facilitating informed decision-making regarding stock levels, replenishment strategies, and resource allocation.

Key Features:

Inventory Simulation: Utilizes DES to create realistic models of inventory processes, capturing complexities such as demand variability, lead times, and restocking policies.

Optimization Techniques: Employs Genetic Algorithms to determine optimal inventory parameters, including reorder points and order quantities, aiming to minimize costs and prevent stockouts.

Performance Optimization: Incorporates Numba, a just-in-time compiler for Python, to accelerate computational tasks, ensuring efficient handling of large-scale simulations.

Interactive User Interface: Features a web-based interface built with Streamlit, allowing users to input parameters, run simulations, and visualize outcomes seamlessly.

API Integration: Provides a FastAPI backend to serve simulation results, enabling easy integration with other systems and facilitating automated workflows.

Repository Structure:

Simulation Modules:

discrete_event_simulation/: Contains scripts and modules for setting up and running DES models of inventory systems.
gen_algo_simulation/: Houses components related to the implementation of Genetic Algorithms for optimizing inventory parameters.
API Services:

des_simulation_api.py: Defines FastAPI endpoints to execute DES simulations and retrieve results programmatically.
des_simulation_opt_api.py: Offers API services focused on optimization tasks using DES models.
gen_single_item_api.py: Provides API endpoints for single-item inventory optimization using Genetic Algorithms.
gen_single_item_opt_api.py: Extends the API services to handle optimization scenarios for single-item inventories.
User Interfaces:

des_simulation_streamlit.py: Streamlit-based application for interactive DES simulation, allowing users to modify parameters and visualize results in real-time.
gen_simulation_streamlit.py: Streamlit interface dedicated to Genetic Algorithm simulations, facilitating user-friendly optimization processes.
Configuration and Dependencies:

requirements.txt: Lists all necessary Python packages and dependencies required to set up and run the project seamlessly.
.gitignore: Specifies files and directories to be excluded from version control, maintaining a clean repository.
Installation and Usage:

Clone the Repository:

bash
Copy
Edit
git clone https://github.com/Asad1287/Inventory-Optimization-with-DES-simulation-and-Genetic-Algorithms.git
cd Inventory-Optimization-with-DES-simulation-and-Genetic-Algorithms
Install Dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run Simulations and Optimizations:

DES Simulation Interface:

bash
Copy
Edit
streamlit run des_simulation_streamlit.py
Access the interactive simulation dashboard via the provided local URL.

DES Simulation API:

bash
Copy
Edit
uvicorn des_simulation_api:app --reload
Launches the FastAPI server to handle DES simulation requests.

Genetic Algorithm Optimization API:

bash
Copy
Edit
uvicorn gen_single_item_opt_api:app --reload
Starts the API service for single-item inventory optimization using Genetic Algorithms.

This project stands as a valuable resource for professionals and researchers in inventory management, offering advanced tools to simulate and optimize inventory systems effectively.
