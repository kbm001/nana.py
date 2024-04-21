# nana.py
import streamlit as st

def find_largest(a, b, c):
    largest = max(a, b, c)
    return largest

def main():
    st.title('Find the Largest Among Three Numbers')
    
    st.write("Enter three numbers below:")
    a = st.number_input("Enter the first number", value=0)
    b = st.number_input("Enter the second number", value=0)
    c = st.number_input("Enter the third number", value=0)
    
    if st.button("Find Largest"):
        largest = find_largest(a, b, c)
        st.write(f"The largest number among {a}, {b}, and {c} is: {largest}")

if __name__ == "__main__":
    main()
