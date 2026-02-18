{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyOzgqHtdvjTLJBNIb0bEX9E",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/JuiiiDixit/Jui-Dixit-EDA-AllExpts-25070123059/blob/main/Study_of_numpy_library.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "#Experiment number 8\n",
        "##Tools for EDA- Study of Numpy library\n",
        "\n",
        "##Name: Jui Dixit\n",
        "##Class: ENTC A3\n",
        "##PRN: 25070123059\n",
        "##Date: 18/2/2026"
      ],
      "metadata": {
        "id": "9JoAo7VZLlB2"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "##Numpy is used to create arrays and perform numerical operations"
      ],
      "metadata": {
        "id": "Xp9aWRMQMQjY"
      }
    },
    {
      "cell_type": "code",
      "execution_count": 3,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "b6pGh-jBLMzM",
        "outputId": "ea5e7836-db36-4dc3-cad3-39769c1acebb"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[10 20 30 40]\n",
            "[[1 2 3]\n",
            " [4 5 6]]\n"
          ]
        }
      ],
      "source": [
        "#Declaration of numpy\n",
        "import numpy as np\n",
        "a = np.array([10, 20, 30, 40])\n",
        "b = np.array([[1,2,3], [4,5,6]])\n",
        "print(a)\n",
        "print(b)"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Dimension of array\n",
        "print(a.ndim)\n",
        "print(b.ndim)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "D5NZoIdoNjUJ",
        "outputId": "829624d3-8ad6-4d10-d44d-8a81baba7589"
      },
      "execution_count": 4,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1\n",
            "2\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(a.shape)\n",
        "print(b.shape)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "sbf7dkQeNtQX",
        "outputId": "42b4c1b3-9b81-45f1-976b-22086a4032b4"
      },
      "execution_count": 5,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "(4,)\n",
            "(2, 3)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(a.dtype)\n",
        "print(b.dtype)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "y1RdYuv6OdDY",
        "outputId": "4b4f2d1d-78de-4d40-ad27-9e2f58eb3671"
      },
      "execution_count": 6,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "int64\n",
            "int64\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Inbuilt functions using numpy\n",
        "print(np.zeros((2,3)))\n",
        "print(np.ones((3,3)))\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "g7KcRkEHOr24",
        "outputId": "fbe95bda-5a0b-45b9-c45f-21fa03c295d7"
      },
      "execution_count": 12,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[[0. 0. 0.]\n",
            " [0. 0. 0.]]\n",
            "[[1. 1. 1.]\n",
            " [1. 1. 1.]\n",
            " [1. 1. 1.]]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(np.eye((3))) #supports only symmetric matrix,so write 3 only once"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "goaGD3a4PUvo",
        "outputId": "94906d3f-9176-404e-d5a3-62620309857a"
      },
      "execution_count": 15,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[[1. 0. 0.]\n",
            " [0. 1. 0.]\n",
            " [0. 0. 1.]]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(np.arange(1,10,2))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "v4SODgiEPgvQ",
        "outputId": "1d4964e7-7c6f-4b8f-be89-6d4df964c313"
      },
      "execution_count": 19,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[1 3 5 7 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "np.linspace(0,6,3)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Yvfyzc0wPv2w",
        "outputId": "26abcd08-3082-4d0f-a9f9-d5e6c2b31064"
      },
      "execution_count": 20,
      "outputs": [
        {
          "output_type": "execute_result",
          "data": {
            "text/plain": [
              "array([0., 3., 6.])"
            ]
          },
          "metadata": {},
          "execution_count": 20
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "c = b*2\n",
        "d = a + 5\n",
        "print(c)\n",
        "print(d)\n",
        "#It is taking the values of a and b as mentioned in the very first code"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "aKF5x14TQDpY",
        "outputId": "142d0cee-c986-40e4-a284-4ae26e2995f7"
      },
      "execution_count": 21,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[[ 2  4  6]\n",
            " [ 8 10 12]]\n",
            "[15 25 35 45]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(np.mean(a))\n",
        "print(np.mean(b))\n",
        "print(np.median(a))\n",
        "print(np.median(b))\n",
        "print(np.max(a))\n",
        "print(np.max(b))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Ey7FFHZVQe_X",
        "outputId": "a2a65544-9305-473f-98e0-c797835825a2"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "25.0\n",
            "3.5\n",
            "25.0\n",
            "3.5\n",
            "40\n",
            "6\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print(np.sum(a))\n",
        "print(np.sum(b))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "i991Y2OKTMia",
        "outputId": "e7afab70-2194-481c-fc40-e0f4d8b7f30d"
      },
      "execution_count": 24,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "100\n",
            "21\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [],
      "metadata": {
        "id": "uZ2-gxsKTUZB"
      },
      "execution_count": null,
      "outputs": []
    }
  ]
}
