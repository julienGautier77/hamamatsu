# hamamatsu


pvCam camera control is an user interface to control Photometrics scientifics camera

This software is not associated with Photometrics . Use it at your own risk.

it use hamamatsu library from  https://github.com/tiagocoutinho/hamamatsu

It can make plot profile and data measurements analysis by using : https://github.com/julienGautier77/visu

It is tested :
on win 11 64 bits (AMD64) with python 3.9.7 MSC v.1916 with 64 bits mini conda installation on aorcaa

Requirements
python 3.x
Numpy
PyQt6
visu

Installation

   hamamatsu

   pip install hamamatsu for installing https://github.com/tiagocoutinho/hamamatsu

   Install visu :

   pip install git+https://github.com/julienGautier77/visu

Usage
appli = QApplication(sys.argv)
   
appli.setStyleSheet(qdarkstyle.load_stylesheet(qt_api='pyqt6'))
e = HAMAMATSU(camID=None)  
e.show()
appli.exec_() 
