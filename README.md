import streamlit as st

# Theme configuration
st.set_page_config(page_title="Blue Falcon Online", page_icon="🦅")

# Blue Falcon Branding
st.markdown("""
    <style>
    .stApp { background-color: #f8f9fa; }
    h1 { color: #1E3A8A; }
    .stButton>button { background-color: #1E3A8A; color: white; border-radius: 20px; }
    </style>
    """, unsafe_allow_html=True)

st.image("https://images.unsplash.com/photo-1544911845-1f34a3eb46b1?q=80&w=200", width=150) # Temporary Falcon Image
st.title("Blue Falcon Enterprise")
st.info("Now Live & Searchable Online")

# Business Logic
service = st.selectbox("Select a Falcon Service", ["Consulting", "Tech Setup", "Maintenance"])
if st.button("Get Instant Quote"):
    st.write(f"Your custom quote for **{service}** is being processed!")

