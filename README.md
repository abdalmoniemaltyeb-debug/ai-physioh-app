# ai-physioh-app
Applications to monitoring ex progam
import streamlit as st

st.set_page_config(
    page_title="AI Physiotherapy",
    page_icon="💪",
    layout="wide"
)

# Header
st.title("💪 AI Physiotherapy Monitoring System")
st.subheader("Smart Home Exercise Tracking Using Artificial Intelligence")

st.write("---")

# About
st.header("📖 About The System")
st.write(
    "This AI-based system helps patients perform physiotherapy exercises "
    "correctly at home using artificial intelligence and camera tracking."
)

# Features
st.header("✨ Features")
st.write("✔ Real-time exercise monitoring")
st.write("✔ AI posture detection")
st.write("✔ Home physiotherapy support")
st.write("✔ Correct / Incorrect feedback")

# Exercise Section
st.header("🏃 Supported Exercises")
exercise = st.selectbox(
    "Choose Exercise",
    ["Shoulder Exercise", "Back Exercise", "Neck Exercise"]
)

st.success(f"{exercise} selected successfully")

# Camera Section
st.header("📷 Camera Monitoring")

start = st.button("Start Monitoring")

if start:
    st.info("Camera and AI monitoring will start here")

# Footer
st.write("---")
st.caption("Developed for Physiotherapy Research Project")
