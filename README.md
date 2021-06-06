# crop-combine-python
import cv2
import  numpy
iron=cv2.imread("<image name>")
cap=cv2.imread("<image name>")
cropcp=cap[:150,:]
cropcpa=cropcp[:,: 120]
cv2.imshow("f1", cropcpa)
cv2.waitKey()
cv2.destroyAllWindows()
cropio=iron[:150,75:-76]
cropioa=cropio[:,77:]
cv2.imshow("io", cropioa)
cv2.waitKey()
cv2.destroyAllWindows()
iocp=numpy.hstack((cropcpa , cropioa))
cv2.imshow("io",iocp)
cv2.waitKey()
cv2.destroyAllWindows()
