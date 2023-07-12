
# DDoS Detection

## Description

A Distributed Denail-of-Service (DDoS) attack is a malicious attempt to disrupt the normal traffic of a targeted server, service or network by overwhelming the target or its surrounding infrastructure with a flood of Internet traffic.

There are different ways to prevent these attacks, but none of them can be cent-percent accurate, our motive is to design a firewall for avoiding DDoS attacks. For that, accurate detection of the attack is essential.

In this proposed system, we are using multiple machine learning-based algorithms to detect DDoS attack.
## Run Locally

Clone the project
```bash
  git clone https://github.com/MidanAhmed/ddos-detection.git
```

Open the project directory in Jupyter Notebook, the following files must be present:
* `main.ipynb`
* `generateCSV.ipynb`
* `gui.ipynb`
* `dataset.csv`

Run the `generateCSV.ipynb` file to split `dataset.csv` to different sections and generate following files:
* `data10000.csv`
* `data12000.csv`
* `data14000.csv`
These files are used for testing purposes.

Once the sectioned datasets have been generated, run `main.ipynb` to train the model on the dataset, namely `dataset.csv`.

The model will be then trained on a particular machine learning algorithm and a `.joblib` file will be created.

The following files will be created for the respective algorithms:
| Trained algorithm        | File generated |
| -----------------        | -------------- |
| Logistic Regression      | `logisticr.joblib` |
| Decision Tree Classifier | `decisiont.joblib` |
| Random Forest Classifier | `randomf.joblib`   |
| Gaussian Naive Bayes     | `naiveb.joblib`    |

Start the Graphical User Interface (GUI) by running `gui.ipynb` and selecting the file to be tested.


## Screenshots

![App Screenshot]([https://via.placeholder.com/468x300?text=App+Screenshot+Here](https://github.com/MidanAhmed/ddos-detection/blob/da6ad4012bcd11e0cbad0c848b98e0046a98b721/image.png))

![App Screenshot 1]([https://via.placeholder.com/468x300?text=App+Screenshot+Here](https://github.com/MidanAhmed/ddos-detection/blob/da6ad4012bcd11e0cbad0c848b98e0046a98b721/image1.png))


## Tech Stack Used

This project has been implemented in the Jupyter.
Major python libraries involved in faster implementation are listed below:
* numpy
* pandas
* scikit-learn
* tkinter


## Acknowledgement

I would like to take this opportunity to express my gratitude to all of my group members **Kishor Kumar Hazarika**, **Ruhul Amin Talukdar** and **Zakaria Ahmed Laskar**. The project would not have been successful without their cooperation and inputs.
