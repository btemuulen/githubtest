# githubtest

 "cells": [
  {
   "cell_type": "code",
   "execution_count": 37,
   "id": "89164f19",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[ 50  51  52  53  54  55  56  57  58  59  60  61  62  63  64  65  66  67\n",
      "  68  69  70  71  72  73  74  75  76  77  78  79  80  81  82  83  84  85\n",
      "  86  87  88  89  90  91  92  93  94  95  96  97  98  99 100]\n"
     ]
    }
   ],
   "source": [
    "#1\n",
    "data1=np.arange(50, 101)\n",
    "print(data1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 36,
   "id": "10a14e38",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n",
      "[[2 2 2 2 2 2 2 2 2 2]]\n",
      "[[6 6 6 6 6 6 6 6 6 6]]\n"
     ]
    }
   ],
   "source": [
    "#2\n",
    "data=np.ones(10)\n",
    "data1=[2,2,2,2,2,2,2,2,2,2]\n",
    "data2=[6,6,6,6,6,6,6,6,6,6]\n",
    "\n",
    "print(data)\n",
    "\n",
    "a=np.array([data1])\n",
    "print(a)\n",
    "\n",
    "b=np.array([data2])\n",
    "print(b)\n",
    "\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 62,
   "id": "fa0ef8eb",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[[20 21 22 23]\n",
      " [24 25 26 27]\n",
      " [28 29 30 31]]\n"
     ]
    }
   ],
   "source": [
    "#3\n",
    "c=np.arange(20, 32)\n",
    "c1=np.reshape(a, (3, 4), \"c\")\n",
    "print(c1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 51,
   "id": "31a99f65",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[[1 0 0]\n",
      " [0 1 0]\n",
      " [0 0 1]]\n"
     ]
    }
   ],
   "source": [
    "#4\n",
    "d=[1,0,0,0,1,0,0,0,1]\n",
    "d1=np.array([d])\n",
    "d2=np.reshape(d1, (3, 3))\n",
    "print(d2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 53,
   "id": "0149e8b7",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[[1 0 0 0 0]\n",
      " [0 2 0 0 0]\n",
      " [0 0 3 0 0]\n",
      " [0 0 0 4 0]\n",
      " [0 0 0 0 5]]\n"
     ]
    }
   ],
   "source": [
    "#5\n",
    "e=[1,0,0,0,0,0,2,0,0,0,0,0,3,0,0,0,0,0,4,0,0,0,0,0,5]\n",
    "e1=np.array([e])\n",
    "e2=np.reshape(e1, (5, 5))\n",
    "print(e2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 60,
   "id": "61144c02",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "32\n"
     ]
    }
   ],
   "source": [
    "#6\n",
    "f=[[6, 10, 5], [1, 3, 7]]\n",
    "f1=np.array(f)\n",
    "print(np.sum(f1))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 79,
   "id": "c087c4b1",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "136\n",
      "[[12 15 16 17  1]\n",
      " [ 2  3  9 56  5]]\n",
      "[[14 18 25 73  6]]\n"
     ]
    }
   ],
   "source": [
    "#6\n",
    "z=[[12, 15, 16, 17, 1], [2, 3, 9, 56, 5]]\n",
    "z1=np.array([z])\n",
    "print(np.sum(z1))\n",
    "print(z1.sum(axis=0))\n",
    "print(z1.sum(axis=1))\n",
    "\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 75,
   "id": "be93f3cc",
   "metadata": {
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[189711742 205782921 204790923 222427819 207376342 187315992 177390145\n",
      " 128190300 133568382 131625891]\n",
      "[106802954 111060153 297968177 170645536 160386023 155317800 271772916\n",
      " 273423453 127333176 113470269]\n",
      "[663 596 531 705 547 514 333 314 338 274]\n",
      "[185 446 667 602 608 250 663 543 393 458]\n",
      "[14716 13072 10704 13596 10239  9078  6687  5246  5358  4683]\n",
      "[ 4159  5650 17675 12211  7927  4451 11719 15040  6372  8175]\n"
     ]
    }
   ],
   "source": [
    "#7\n",
    "#Salaries\n",
    "KobeBryant_Salary = [27849149,30453805,23500000,25000000,0,0,0,0,0,0]\n",
    "JoeJohnson_Salary = [19752645,21466718,23180790,25309344,11000000,9978835,220000,0,0,151821]\n",
    "LeBronJames_Salary = [17545000,19067500,20644400,22971000,30963450,33285709,35654150,37436858,39219566,41180544]\n",
    "CarmeloAnthony_Salary = [19450000,22407474,22458000,22875000,24559380,26243760,25534253,2393887,2159029,2564753]\n",
    "DwightHoward_Salary = [19536360,20513178,21436271,22359364,23180275,23500000,18919725,5337000,3039097,2564753]\n",
    "ChrisBosh_Salary = [17545000,19067500,20644400,22192730,23741060,25289390,26837720,0,0,0]\n",
    "ChrisPaul_Salary = [17779458,18668431,20068563,21468696,22868827,24599495,35654150,38506482,41358814,30800000]\n",
    "KevinDurant_Salary = [16669630,17832627,18995624,20158622,26540100,25000000,30000000,37199000,40108950,40918900]\n",
    "DerrickRose_Salary = [16402500,17632688,18862875,20093063,21323250,2397421,2176260,7317073,7682926,13445120]\n",
    "DwayneWade_Salary = [17182000,18673000,15000000,20000000,23200000,17021382,2393887,0,0,0]\n",
    "#Matrix\n",
    "Salary = np.array([KobeBryant_Salary, JoeJohnson_Salary, LeBronJames_Salary, CarmeloAnthony_Salary, DwightHoward_Salary, ChrisBosh_Salary, ChrisPaul_Salary, KevinDurant_Salary, DerrickRose_Salary, DwayneWade_Salary])\n",
    "\n",
    "#Games \n",
    "KobeBryant_G = [78,6,35,66,0,0,0,0,0,0]\n",
    "JoeJohnson_G = [72,79,80,81,78,55,0,0,0,1]\n",
    "LeBronJames_G = [76,77,69,76,74,82,55,67,45,46]\n",
    "CarmeloAnthony_G = [67,77,40,72,74,78,10,58,69,57]\n",
    "DwightHoward_G = [76,71,41,71,74,81,9,69,69,47]\n",
    "ChrisBosh_G = [74,79,44,53,0,0,0,0,0,0]\n",
    "ChrisPaul_G = [70,62,82,74,61,58,58,70,70,58]\n",
    "KevinDurant_G = [81,81,27,72,62,68,78,0,35,39]\n",
    "DerrickRose_G = [0,10,51,66,64,25,51,50,50,26]\n",
    "DwayneWade_G = [69,54,62,74,60,67,72,0,0,0]\n",
    "#Matrix\n",
    "Games = np.array([KobeBryant_G, JoeJohnson_G, LeBronJames_G, CarmeloAnthony_G, DwightHoward_G, ChrisBosh_G, ChrisPaul_G, KevinDurant_G, DerrickRose_G, DwayneWade_G])\n",
    "\n",
    "#Points\n",
    "KobeBryant_PTS = [2133,83,782,1161,0,0,0,0,0,0]\n",
    "JoeJohnson_PTS = [1170,1245,1154,992,715,372,0,0,0,2]\n",
    "LeBronJames_PTS = [2036,2089,1743,1920,1954,2251,1505,1698,1126,1353]\n",
    "CarmeloAnthony_PTS = [1920,2112,966,1573,1659,1261,134,895,924,767]\n",
    "DwightHoward_PTS = [1296,1297,646,976,1002,1347,115,517,482,249]\n",
    "ChrisBosh_PTS = [1232,1281,928,1010,0,0,0,0,0,0]\n",
    "ChrisPaul_PTS = [1186,1185,1564,1446,1104,1081,906,1232,1149,866]\n",
    "KevinDurant_PTS = [2280,2593,686,2029,1555,1792,2027,0,943,1135]\n",
    "DerrickRose_PTS = [0,159,904,1080,1154,209,917,904,734,311]\n",
    "DwayneWade_PTS = [1463,1028,1331,1409,1096,765,1083,0,0,0]\n",
    "#Matrix\n",
    "Points = np.array([KobeBryant_PTS, JoeJohnson_PTS, LeBronJames_PTS, CarmeloAnthony_PTS, DwightHoward_PTS, ChrisBosh_PTS, ChrisPaul_PTS, KevinDurant_PTS, DerrickRose_PTS, DwayneWade_PTS])             \n",
    "                  \n",
    "print(Salary.sum(axis=0))   \n",
    "print(Salary.sum(axis=1))\n",
    " \n",
    "print(Games.sum(axis=0))   \n",
    "print(Games.sum(axis=1))\n",
    "\n",
    "print(Points.sum(axis=0))   \n",
    "print(Points.sum(axis=1))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 80,
   "id": "f7a1dea2",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "\f",
      "\n"
     ]
    }
   ],
   "source": []
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "d7edc02a",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
Footer
© 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
