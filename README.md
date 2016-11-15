# SM_Lab12-2016179-
#swagger
def insert(a):
	for i in range(1,len(a),1):
		s=a[i]
		p=0
		print ('ho')
		for j in range(i-1,-1,-1):
			print (i,j,'lo')
			if (a[j]>s):
				print ('yes',a[j],a[j+1])
				a[j+1]=a[j]
				print ('yes',a[j],a[j+1])
				p=1
			else :
				break
		if(i==1 and p==1):		
			a[j]=s
		else:
			a[j+1]=s
		print (a)
	return a
  
print (insert([2,1,11,4,57,64,0,98,7]))
