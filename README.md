# reading-text-file-

# Read text from a file, and count the occurence of words in that text
# Example:
# count_words("The cake is done. It is a big cake!")
# --> {"cake":2, "big":1, "is":2, "the":1, "a":1, "it":1}

#first access the file path
file = open('C:/Users/Mlolaiya/story.txt', 'r')
content = file.read()

#HOW TO ACCESS NUMBER OF OCCURENCE OF WORDS IN PYTHON
def read_file_content(content):
#to read text-file, pass a file name
   content = file.read()

    return content

print(content) #This will print out the text-file


def count_words(content):
    counts = dict()
    text = content.split()

    for word in text:
        if word in counts:
            counts[word] += 1
        else:
            counts[word] = 1

    return counts

print(count_words('Once upon a time a psychology professor walked around on a stage while teaching stress management principles to an auditorium '
                  'filled with students. As she raised a glass of water, everyone expected they would be asked the typical glass half empty or glass'
                  ' half full question. Instead, with a smile on her face, the professor asked, How heavy is this glass of water I am holding?'))
