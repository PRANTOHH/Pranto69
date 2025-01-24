import React, { useState } from "react";

const PlayerInterface = () => {
  const [sentCount, setSentCount] = useState(100);

  const handleSent = () => {
    setSentCount((prevCount) => prevCount + 1);
  };

  return (
    <div style={{ fontFamily: "Arial, sans-serif", textAlign: "center", marginTop: "50px" }}>
      <h1>Player Sent Interface</h1>
      <h2>Sent: {sentCount}+</h2>
      <button
        onClick={handleSent}
        style={{
          padding: "10px 20px",
          fontSize: "16px",
          cursor: "pointer",
          backgroundColor: "#4CAF50",
          color: "white",
          border: "none",
          borderRadius: "5px",
        }}
      >
        Send
      </button>
    </div>
  );
};

export default PlayerInterface;
