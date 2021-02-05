def josephus(number):
	queue = []
	queue.extend(range(1, number + 1))
	while len(queue) > 1:
		queue.append(queue[0])
		queue.pop(0)
		queue.pop(0)
	return queue


def josephus2(number):
	a = bin(number)
	l = number - 2 ** (len(a) - 3)
	solution = l * 2 + 1
	x = [solution]
	return x


def proof(number):
	wrong = 0
	correct = 0
	for i in range(1, number + 1):
		if josephus(i) == josephus2(i):
			correct += 1
		else:
			wrong += 1
	print("correct:", correct)
	print("wrong:", wrong)
