# Test

# Prompt List with Copy Button

아래 버튼을 누르면 프롬프트가 클립보드에 복사됩니다.

<div style="border:1px solid #ddd; padding:10px; border-radius:6px; margin-bottom:1em;">
  <pre id="prompt1">You are a helpful AI assistant that answers in detail.</pre>
  <button onclick="copyToClipboard('prompt1')">📋 Copy</button>
</div>

<div style="border:1px solid #ddd; padding:10px; border-radius:6px; margin-bottom:1em;">
  <pre id="prompt2">Generate 10 blog post ideas about AI in healthcare.</pre>
  <button onclick="copyToClipboard('prompt2')">📋 Copy</button>
</div>

<script>
function copyToClipboard(elementId) {
  const text = document.getElementById(elementId).innerText;
  navigator.clipboard.writeText(text).then(() => {
    alert("✅ Copied to clipboard!");
  });
}
</script>
